# Compliment Bot

Compliment Bot — Telegram-бот, который создает комплименты на основе того, что пользователю нравится в девушке. Использует API Gemini и поддерживает прокси.

## Описание проекта

Бот написан на Python с `python-telegram-bot`. Генерирует комплименты через API Gemini и поддерживает SOCKS5-прокси.

## Установка и запуск

### 1. Клонирование репозитория

Склонируйте репозиторий на локальную машину:

```bash
git clone https://github.com/KrutilinNikita/Compliment_bot.git
cd Compliment_bot
```

### 2. Создание виртуального окружения (рекомендуется)

```bash
python3 -m venv venv
source venv/bin/activate  # Для Windows используйте venv\Scripts\activate
```

### 3. Установка зависимостей

```bash
pip install -r requirements.txt
```

### 4. Настройка переменных окружения

Создайте файл `.env` в корневой директории на основе `.env.template` и заполните его:

```
GEMINI_API_KEY=your_gemini_api_key
TELEGRAM_TOKEN=your_telegram_token
PROXY=socks5h://username:password@host:port
```

- **`GEMINI_API_KEY`** — ключ API для доступа к Gemini.
- **`TELEGRAM_TOKEN`** — токен бота в Telegram (получить через [BotFather](https://t.me/BotFather)).
- **`PROXY`**  — прокси для работы бота, если он недоступен без VPN.

### 5. Запуск бота

```bash
python compliment_bot/main.py
```

### 6. Примечание

Для проверки корректности работы:

```bash
python -m unittest discover -s tests
```

## Контакты

Если у вас есть вопросы или предложения, пишите на [nikita.krutilin@example.com](mailto:nikita.krutilin@example.com).
