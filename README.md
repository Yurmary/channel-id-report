# 📊 Channel ID Report

> Автоматический отчёт для сверки идентификаторов товаров между каналами продаж (Wildberries, Ozon, Amazon и др.) и базой 1С. Результаты сохраняются в Excel и отправляются в Telegram.

## 🚀 Что делает скрипт

- Подключается к PostgreSQL
- Выполняет SQL-запросы для разных маркетплейсов
- Сравнивает внешний ID с ID в 1С
- Генерирует Excel-отчёт с цветными вкладками
- Отправляет результат в Telegram

## 📦 Используемые технологии

- Python (pandas, openpyxl, psycopg2)
- PostgreSQL
- Telegram Bot API
- Cron (для запуска по расписанию)

## ⚙️ Как использовать

1. Установи зависимости:
```bash
pip install -r requirements.txt

2. Заполни параметры подключения и токены в weekly_report.py

3. Запусти: python weekly_report.py

📅 Автоматизация

Можно запускать автоматически раз в неделю через cron:

0 9 * * 1 /usr/local/bin/python3 /Users/твоя_папка/weekly_report.py

👩‍💻 Автор

@Yurmary 