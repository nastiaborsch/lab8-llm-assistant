---
title: LLM Text Assistant
emoji: 📝
colorFrom: indigo
colorTo: blue
sdk: gradio
app_file: app.py
pinned: false
---

# Лабораторна робота №8 — LLM проєкт (базовий рівень)

Вебзастосунок для сумаризації, перекладу, виправлення помилок і спрощення текстів.
Для кожного виконання задачі відправляється один запит до LLM `openai/gpt-oss-20b` через Groq.
Користувач отримує лише кінцевий текст без вступів і пояснень.

## Локальний запуск

```bash
python -m pip install -r requirements.txt
python app.py
```

Відкрийте адресу, яку покаже Gradio (зазвичай `http://127.0.0.1:7860`).
Під час використання введіть власний API-ключ Groq у поле інтерфейсу.
Альтернативно налаштуйте змінну середовища `GROQ_API_KEY`.

## Публікація на Hugging Face Spaces

1. Створіть Space, обравши SDK `Gradio`.
2. Завантажте файли `app.py`, `requirements.txt` і `README.md`.
3. У `Settings` → `Variables and secrets` додайте Secret з назвою `GROQ_API_KEY` для публічного демо без необхідності вводити ключ.
4. Після успішного запуску відкрийте посилання свого Space й перевірте обробку тексту.

Не вставляйте секретний API-ключ у код або README.
