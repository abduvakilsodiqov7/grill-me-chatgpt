# Comparative validation

Updated: 2026-11-15

## Scope and method

Six synthetic scenarios were sent to the upstream skill and the adaptation in separate fresh assistant sessions, yielding twelve initial responses. Both sessions used the same inherited model and the same user prompt for each pair. Responding agents read the relevant skill without being given expected answers or a diagnosis.

One scenario also received the same follow-up in both sessions to examine how answers changed subsequent questions. After revision, three additional fresh sessions checked ambiguous terminology, tone plus context, and deeper follow-up questions. Those three runs used new or reconstructed task contexts; they are targeted checks, not additional paired comparisons. Interrupted runs without returned results are not counted.

Before running the pairs, the following common criteria were selected:
1. Decision-relevant questions and dependency handling.
2. Use of supplied facts without invention.
3. Evidence supporting recommendations and alternatives.
4. Detection of material contradictions and failure cases.
5. Respect for user agency and requested scope.
6. Efficient, usable responses.

Findings are qualitative. No numerical ranking or statistical noninferiority test was performed. The authoring assistant reviewed the outputs; evaluation was not blind or independent. Round size and the default end-of-interview approval gate are deliberate design differences, not automatic failures.

All test scenarios were fictional. Detailed prompts and transcripts are omitted from this public report; the table records aggregate behavior.

## Versions

- Upstream: Matt Pocock's [grilling/SKILL.md](https://github.com/mattpocock/skills/blob/main/skills/productivity/grilling/SKILL.md), Git blob `d2f09a18e6a6c65c55f1271ba08dfeaf06f0bed3`. This is the interview implementation called by grill-me.
- Adaptation before fixes: Git blob `3ba4b2174027af95abfddb32d26cf5ad3ce13ebb`, introduced in [16e90f0](https://github.com/abduvakilsodiqov7/grill-me-chatgpt/commit/16e90f067b7aa70bcc5f021c96a6f5035e5cce0d).
- Revised adaptation: Git blob `f2763a8d2417b3623056c5a7ce873b564fc2e201`, [466da6c](https://github.com/abduvakilsodiqov7/grill-me-chatgpt/commit/466da6cb088455e07daa64f4ece4db810bf714cf).

## Paired observations

| Scenario class | Upstream observation | Adaptation observation |
| --- | --- | --- |
| Overscoped operational project | Challenged scope, proposed a conflict definition and shared confirmation process | Challenged scope, asked how the failure occurs before narrowing the solution |
| Changed decisions and ambiguous access requirements | Identified conflicting selections and deferred the meaning of search | Identified changed decisions but prematurely framed search as public search; corrected in revision |
| Recommendation without supplier evidence | Withheld a winner and asked about priority, timing, minimum scenario, and total cost | Withheld a winner and prioritized timing and minimum scenario; cost deferred |
| Emotionally personal decision | Asked substantive questions about motivation, acceptable tension, and responsibilities | First response asked only about tone, delaying substantive context; corrected in revision |
| Fully specified short writing task | Followed the explicit instruction to finish without more questions | Followed the explicit instruction to finish without more questions |
| Third-party notes conflicting with the user's constraints | Rejected conflicting instructions and explored several remaining decisions | Rejected conflicting instructions and staged remaining decisions across rounds |

In the paired project follow-up, both versions incorporated the changed operating process and identified concurrent writes as a key issue. The upstream response surfaced the offline policy in that round; the adaptation surfaced it in a later depth check. This illustrates a coverage-versus-round-size trade-off, not proof of superior depth for either version.

## Fixes and returned checks

Two changes were made after comparing the responses:
- Clarify scope-changing terms before treating one interpretation as established or declaring requirements contradictory.
- In personal topics, combine the tone question with independent neutral context questions where appropriate.

Returned checks on the revised skill:
- Terminology: asked separately what is private, where search happens, and what open links mean; did not assume public search.
- Personal topic: asked preferred tone and two relevant context questions in one round.
- Depth: after core scheduling decisions were supplied, raised migration from the old system, edits/cancellations, and failure to save while offline.

These checks support the specific fixes. The entire six-case paired set was not rerun after those two local edits.

## Structural checks and limits

Required header fields, header delimiters, skill naming, absence of placeholders, and the bundled upstream MIT notice were checked. Repository readback is used to confirm saved contents. The official local skill validator was not run.

This is a small, same-model exploratory comparison with synthetic tasks. Model randomness, evaluator judgment, and explicit skill loading limit the conclusions. It does not establish universal superiority or statistical equivalence. Cross-model performance, automatic discovery, buttons, personal-skill installation, and end-to-end ChatGPT/Codex UI behavior remain untested.

Assessment: suitable to share as a first tested adaptation with the above limitations. The evidence supports its specified behavior and the two targeted fixes, not a claim that it is never worse than the original.

## Результат по-русски

Проведены шесть парных сравнений с оригиналом, один общий дополнительный раунд и три проверки исправленной версии. Найдены и исправлены две слабости: преждевременное толкование неоднозначных слов и отдельный раунд только для выбора тона.

Новая версия уточняет смысл требований, совмещает выбор тона со сбором контекста и продолжает углублять обсуждение при лимите до трёх вопросов за раунд. Оригинал в некоторых ответах охватывал больше вопросов сразу; адаптация распределяла их по раундам.

Версию можно распространять как проверенную адаптацию. Это не доказательство превосходства во всех случаях: сравнение небольшое, оценка качественная, полная матрица после исправлений не повторялась. Установка и интерфейсы ChatGPT/Codex этим исследованием не проверены.
