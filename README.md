# 📊 Channel ID Report

> Автоматический отчёт для сверки идентификаторов товаров между каналами продаж (Wildberries, Ozon, Amazon и др.) и базой 1С. Результаты сохраняются в Excel и отправляются в Telegram.

## 🚀 Что делает скрипт

- Подключается к PostgreSQL
- Выполняет SQL-запросы для разных маркетплейсов
- Сравнивает внешний ID с ID в 1С
- Генерирует Excel-отчёт с цветными вкладками
/Users/mary/Downloads/Screenshot at Apr 02 23-33-45.png
- Отправляет результат в Telegram
/var/folders/17/y1m23fh12x150dhn9ff66bfw0000gn/T/com.apple.useractivityd/shared-pasteboard/items/3CC5E45C-0025-44BF-81AB-86C18089B786/IMG_3145.png

## 📦 Используемые технологии

- Python (pandas, openpyxl, psycopg2)
- PostgreSQL
- Telegram Bot API
- Cron (для запуска по расписанию)

## ⚙️ Как использовать

1. Установи зависимости:
```bash
pip install -r requirements.txt
```

2. Заполни параметры подключения и токены в weekly_report.py

3. Запусти: 
```bash
python weekly_report.py
```
📅 Автоматизация

Можно запускать автоматически раз в неделю через cron:

```bash
0 9 * * 1 /usr/local/bin/python3 /Users/твоя_папка/weekly_report.py
```
👩‍💻 Автор

@Yurmary 