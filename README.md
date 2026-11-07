<h1 align="center">Ярослав Зайцев</h1>
<p align="center">
  Python-разработчик · AI-инженер · Самара (готов к переезду)<br>
  Делаю Telegram-ботов, бэкенды на FastAPI и системы, где ИИ-агенты работают с реальными инструментами
</p>

<p align="center">
  <a href="https://t.me/pazrabi"><img src="https://img.shields.io/badge/Telegram-@pazrabi-26A5E4?logo=telegram&logoColor=white" alt="Telegram"></a>
</p>

---

### Обо мне

- Квалификация «программист» (Колледж связи ПГУТИ, 2025) и курс Python на 144 часа.
- Строю проекты на связке «я + ИИ-агенты»: ставлю задачи, проверяю код, принимаю ветки, пишу тесты и деплою на свой VPS.
- Мне интересна прикладная разработка с ИИ: MCP-серверы, агенты, автоматизация рутинных процессов в бизнесе.

### Стек

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Telegram Bot API](https://img.shields.io/badge/Telegram_Bot_API-26A5E4?logo=telegram&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)
![Caddy](https://img.shields.io/badge/Caddy-1F88C0?logo=caddy&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=githubactions&logoColor=white)

**ИИ:** MCP (Model Context Protocol), Claude Code, Gemini CLI, оркестрация агентов, LLM как запасной парсер

### Проекты

| Проект | Что это | Технологии |
|---|---|---|
| **[aviaticket](https://github.com/pazrabi/aviaticket)** | Telegram-бот, который ищет дешёвые авиабилеты сразу на 6 сайтах (Aviasales, Яндекс Путешествия, Туту, Купибилет, OZON Travel, Т-Путешествия). Парсеры читают JSON-ответы сайтов, бот хранит историю цен и строит прогноз | Python, Playwright, Telegram Bot API, SQLite, pytest (900+ тестов) |
| **[droidhub](https://github.com/pazrabi/droidhub)** | Сервер для удалённого управления Android-телефонами из браузера и для ИИ-агентов через MCP: скриншоты, тапы, ввод текста, разбор UI. Есть токены для разных клиентов, лимиты, аудит, SSO и Telegram-алерты о перегреве | FastAPI, ADB, Tailscale, MCP, vanilla JS |
| **[gemini-pool](https://github.com/pazrabi/geminipool)** | Пул ИИ-агентов-разработчиков: получает задачу по MCP, агент пишет код в отдельной git-ветке, второй агент делает ревью и прогоняет тесты, затем отчёт уходит ведущему. Есть веб-дашборд и OAuth | Python stdlib, git worktrees, MCP, OAuth 2.0, systemd |
| **[roulette](https://github.com/pazrabi/roulette)** | Telegram Mini App с мини-играми на виртуальных фишках: экономика, скины-сцены, рефералы, бэкапы с шифрованием | FastAPI, JS, SQLite, GitHub Actions CI, e2e-тесты |

Проекты связаны между собой: агенты из **gemini-pool** пишут код для остальных, **aviaticket** берёт живые цены через телефоны **droidhub**, а всё вместе собрано на одном домене с единым входом.
