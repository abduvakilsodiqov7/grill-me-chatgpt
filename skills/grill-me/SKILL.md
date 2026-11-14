---
name: grill-me
description: Interview the user in rounds to clarify and stress-test a task, plan, idea, or decision. Use when requested with grill-me, grill me, допроси меня, сначала разберись, or similar expressions. For a complex task, offer this workflow first and use it only if the user agrees.
---

# Grill Me

Help the user think through a task before starting it. Adapted from Matt Pocock's [grill-me and grilling](https://github.com/mattpocock/skills/tree/main/skills/productivity) skills, under the MIT license in this repository.

## Activation

- Start on an explicit request, including /grill-me or the trigger phrases above.
- For a complex task with significant unresolved decisions, suggest this workflow; begin it only if the user accepts.
- Follow the user's instruction to shorten the interview, skip questions, or start work.

## Interview

1. First examine the request and accessible context and materials. Do not ask the user to repeat information already available.
2. Identify decisions and uncertainties that could materially change the outcome. Map their dependencies: ask later about decisions that depend on answers still outstanding.
3. Ask up to three independent questions per round, and wait for answers before selecting the next round. Number them so users can reply by number.
4. Where choices make sense, offer clear alternatives and put a recommended answer first, with a brief reason. Make room for a different answer or "I don't know". Avoid forcing a choice where an open question works better.
5. Use interactive choice tools only when available and appropriate; otherwise present ordinary text. Never imply that buttons will always be available.
6. When the user does not know an answer, explain the trade-offs and research facts using available tools or materials where useful. If the answer is still uncertain, suggest a temporary assumption, identify what needs verification, and continue when appropriate.
7. Find facts you can reasonably check yourself; distinguish facts, assumptions, and decisions. Do not invent evidence. Challenge weak assumptions and identify relevant risks respectfully.
8. Adjust the depth and number of rounds to the task. Ask only questions that could materially improve the result. Adapt to requests for one question at a time.
9. Respond in the user's language, plainly and naturally.

## Brief and proceed

When the important decisions are sufficiently clear, present a concise brief as relevant: goal, audience, scope and exclusions, decisions, assumptions, and unresolved risks. Then start the requested work without awaiting another confirmation. If the user has asked to review the brief first, wait for their approval. If an essential decision or permission is required for a particular action, ask before that action. Respect higher-priority instructions and platform limits.
