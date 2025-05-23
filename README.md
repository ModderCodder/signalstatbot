📊 SignalStat Bot — Анализ торговых сигналов из Telegram
SignalStat — это Telegram-бот для автоматического сбора, анализа и ранжирования торговых сигналов из Telegram-каналов (акции, фьючерсы, криптовалюты).

Python
Aiogram
PostgreSQL
Docker

🌟 Возможности

✅ Автоматический сбор сигналов из Telegram-каналов
✅ Парсинг и нормализация (Regex + Pydantic)
✅ Хранение данных в PostgreSQL с историей
📊 Статистика и рейтинги каналов (ROI, win rate)
🔒 Pro-версия: автоследование сигналам через API бирж

🛠 Технологический стек

Backend: Python 3.9+
Фреймворк бота: Aiogram
База данных: PostgreSQL + SQLAlchemy
Кэш: Redis
Парсинг: Regex + Pydantic
Деплой: Docker + Docker-Compose

⚡️ Быстрый старт

1. Клонируйте репозиторий
   
```git clone https://github.com/yourusername/signalstat-bot.git```
```cd signalstat-bot```

2. Настройка окружения

Создайте файл .env на основе .env.example:
```BOT_TOKEN=ваш_токен_бота```
```DB_URL=postgresql://user:password@db:5432/signalstat```
```REDIS_URL=redis://redis:6379/0```

3. Запуск через Docker

```docker-compose up -d --build```

4. Команды бота

/start — приветствие
/add_channel @username — добавить канал
/channels — список каналов
/stats — статистика сигналов

🗂 Структура проекта

```signalstat-bot/```
```├── bot/                  # Основной модуль бота```
```│   ├── handlers/         # Обработчики команд```
```│   ├── middlewares/      # Промежуточное ПО```
```│   └── __main__.py       # Точка входа```
```├── db/                   # Работа с базой данных```
```│   ├── models.py         # SQLAlchemy модели```
```│   └── crud.py           # Запросы к БД```
```├── parser/               # Парсинг сигналов```
```│   └── signal_parser.py  # Regex + Pydantic```
```├── docker-compose.yml    # Конфигурация Docker```
```└── README.md             # Этот файл```

🤝 Как помочь проекту

Fork репозитория
Создайте ветку (git checkout -b feature/your-feature)
Сделайте коммит (git commit -am 'Add some feature')
Запушьте (git push origin feature/your-feature)
Откройте Pull Request
