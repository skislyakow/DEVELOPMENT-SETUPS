# DEVELOPMENT SETUPS

Здесь я храню свои настройки и конфигурации для разработки.

## Что здесь

- **Python.gitignore** — универсальный `.gitignore` для Python-проектов
- **coding-rules.md** — 550 правил написания кода (источник: [dvmn.org](https://dvmn.org/reviews/enhancements/))

## Зачем

Делиться своими настройками с другими проектами и использовать как шаблоны.

## Как использовать

Просто скопируйте нужный файл в корень вашего проекта.

## coding-rules.md

Файл **coding-rules.md** — чек-лист для ревью кода, который можно подключить к AI-ассистентам:

- [opencode](https://opencode.ai) — добавьте в `opencode.json` в секцию `systemPrompt`
- [Cursor](https://cursor.com) — добавьте в настройки проекта (`.cursorrules`)
- [Claude](https://claude.ai) — добавьте в документ проекта или System Prompt
- [Roo Code](https://roo-code.com) — добавьте в Custom Instructions

> Используется для **ревью кода** — поиска типичных ошибок и нарушений стандартов. Правила взяты из [dvmn.org/reviews/enhancements](https://dvmn.org/reviews/enhancements/) (550 правил).

### Пример для opencode (opencode.json)

```json
{
  "systemPrompt": "При написании кода следуй правилам из ./coding-rules.md"
}
```

### Быстрая шпаргалка (топ-20)

| # | Правило |
|---|---------|
| 1 | Называй понятно |
| 2 | Избавляйся от мусора |
| 3 | DRY — не повторяйся |
| 4 | Функции делают одно дело |
| 5 | Магические числа — в константы |
| 6 | Исключения — конкретные |
| 7 | Проверяй ввод |
| 8 | snake_case для переменных |
| 9 | UPPER_CASE для констант |
| 10 | f-strings вместо %s |
| 11 | with open() для файлов |
| 12 | os.path.join() для путей |
| 13 | .get() для словарей |
| 14 | enumerate() для индексов |
| 15 | comprehensions для списков |
| 16 | date/time/datetime — разные типы |
| 17 | docstrings по PEP 257 |
| 18 | Коммиты — атомарные |
| 19 | .gitignore от мусора |
| 20 | Тесты сначала |