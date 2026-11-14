# Grill Me for ChatGPT & Codex

[Русский](#русский) | [English](#english)

<a id="english"></a>
## English

A skill that helps you think through a goal, idea, or project before work begins. It interviews you in short rounds, offers recommendations, and turns your answers into a concise brief.

### How it works

- Explicitly ask for **grill-me**; for complex tasks the assistant may suggest it first.
- Each round has up to three independent questions, with suggested answers where useful.
- The assistant helps research uncertainty and labels assumptions instead of inventing facts.
- Once the main decisions are clear, it presents a brief and starts work. Ask it to wait for your approval if you prefer.
- You can always change an answer, ask for fewer questions, or say “start now.”

Example: **“grill-me: I want to build a website for a café.”**

Interactive buttons, automatic invocation, and exact trigger syntax depend on the product and its available tools. Typed answers work too.

### Use with Codex

Copy the complete [skills/grill-me](skills/grill-me) folder into `.agents/skills/grill-me` in your project, or into `~/.agents/skills/grill-me` for your user account. Start a new session so Codex can discover the skill. You can then ask Codex to use **grill-me**; if the skill is offered in the interface, select it there.

For current details, see [OpenAI's Codex skills documentation](https://developers.openai.com/codex/skills/).

### Use with ChatGPT

Where personal skills are available, open **Plugins → Skills** and use the available create or editor flow to create a skill using the instructions in [SKILL.md](skills/grill-me/SKILL.md). Follow the interface's installation prompts. Availability, upload support, and syncing vary by account, workspace, and product; publishing this repository does not install the skill automatically.

See [Skills in ChatGPT](https://help.openai.com/en/articles/20001066-skills-in-chatgpt). If skills are unavailable, paste the instructions into a conversation and ask ChatGPT to use them for the current task.

### Attribution and license

Adapted from [Matt Pocock's skills](https://github.com/mattpocock/skills), particularly grill-me and grilling. The original MIT copyright and permission notice is retained in [LICENSE](LICENSE).

<a id="русский"></a>
## Русский

Скилл помогает продумать цель, идею или проект до начала работы. Он задаёт вопросы небольшими раундами, предлагает рекомендации и собирает ответы в краткий бриф.

### Как это работает

- Попросите использовать **grill-me**; для сложной задачи помощник может сначала предложить этот режим.
- В каждом раунде — до трёх независимых вопросов. Если уместно, помощник предлагает варианты и рекомендует один из них.
- Если ответа нет, помощник помогает разобраться и отмечает предположения.
- Когда основные решения приняты, он показывает бриф и начинает работу. Если хотите сначала проверить бриф, попросите его дождаться вашего согласия.
- Можно изменить ответ, попросить меньше вопросов или сказать «начинай».

Пример: **«grill-me: хочу сделать сайт для кафе»**.

Кнопки, автоматический запуск и точная команда зависят от продукта и доступных инструментов. Можно отвечать обычным текстом.

### Использование в Codex

Скопируйте папку [skills/grill-me](skills/grill-me) целиком в `.agents/skills/grill-me` внутри проекта или в `~/.agents/skills/grill-me` для своего пользователя. Начните новую сессию, чтобы Codex обнаружил скилл. Затем попросите использовать **grill-me** или выберите его в интерфейсе, если он там отображается.

Подробнее: [документация OpenAI о скиллах в Codex](https://developers.openai.com/codex/skills/).

### Использование в ChatGPT

Если вашему аккаунту доступны персональные скиллы, откройте **Plugins → Skills** и создайте скилл через доступный редактор или чат, используя инструкции из [SKILL.md](skills/grill-me/SKILL.md). Затем следуйте указаниям интерфейса по установке. Доступность, загрузка и синхронизация зависят от аккаунта, рабочего пространства и продукта; публикация на GitHub не устанавливает скилл автоматически.

Подробнее: [скиллы в ChatGPT](https://help.openai.com/ru-ru/articles/20001066-skills-in-chatgpt). Если скиллы недоступны, можно вставить инструкции в чат и попросить применить их к текущей задаче.

### Авторство и лицензия

Адаптация [скиллов Мэтта Покока](https://github.com/mattpocock/skills), в частности grill-me и grilling. Уведомление об авторском праве и условия оригинальной лицензии MIT сохранены в [LICENSE](LICENSE).
