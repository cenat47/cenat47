# Привет, я Максим 👋
### Python Backend Developer

Специализируюсь на создании асинхронных сервисов и API.

---

### 🛠 Технологический стек

*   **Backend:** Python 3.11+ (FastAPI, Asyncio, Pydantic v2)
*   **Databases:** PostgreSQL (SQLAlchemy ORM, Alembic), Redis
*   **Asynchronous Tasks:** Celery, Flower
*   **Infrastructure:** Docker, Docker Compose, Nginx
*   **Testing & Quality:** Pytest, Ruff, MyPy
*   **Tools:** Git

---
### 🏗 Мой подход к архитектуре (используется во всех проектах ниже)
Во всех своих проектах я придерживаюсь принципов **Clean Architecture** и разделения ответственности, что делает код тестируемым и поддерживаемым:

*   **Layered Architecture:** Четкое разделение на роутеры (FastAPI), сервисы (Business Logic) и репозитории (Data Access).
*   **Data Integrity:** Использование **DTO (Pydantic v2)** для валидации входящих данных и фильтрации ответов API.
*   **Database Patterns:** Работа с БД через **SQLAlchemy ORM**, управление миграциями через **Alembic**.
*   **Asynchronous:** Подходящее использование `async/await` и вынос тяжелых задач (отчеты, парсинг) в фоновые очереди **Celery + Redis**.
*   **Environment:** Контейнеризация всего окружения через **Docker Compose** для быстрого развертывания.

---
### 🚀 Мои основные проекты на GitHub

#### 📊 [Report Service](https://github.com/cenat47/CenatReports)  — Сервис генерации отчетов
Backend-система для асинхронного формирования 10+ типов CSV-отчетов с многоуровневой системой безопасности.
*   **Стек:** FastAPI, Celery, Redis, PostgreSQL (SQLAlchemy), Docker.
*   **Security:** JWT-авторизация (Access/Refresh), ротация токенов, RBAC (роли User/Manager/Admin).
*   **Performance:** Вынос тяжелых задач в Celery, оптимизация запросов к БД, обработка ошибок и мониторинг статусов задач.


#### 📈 [crypto_price_tracker](https://github.com/cenat47/crypto_price_tracker) — Асинхронный сервис мониторинга цен 
Система для автоматического сбора и анализа исторических данных котировок (BTC, ETH) с биржи Deribit.
*   **Стек:** FastAPI, Celery, PostgreSQL (SQLAlchemy), aiohttp, Pydantic.
*   **Асинхронность:** Интеграция с внешним API реализована через асинхронный клиент `aiohttp`, сбор данных автоматизирован с помощью Celery-worker.
*   **API:** Реализована гибкая фильтрация исторических данных по временным интервалам и тикерам.


#### 🏨 [Hotel API](https://github.com/cenat47/hotel_api) — Система бронирования с кэшированием
REST API для управления отелями и бронированиями, спроектированное под высокие нагрузки.
*   **Стек:** FastAPI, PostgreSQL, Redis, Pytest, Ruff.
*   **Производительность:** Внедрено кэширование в Redis для мгновенного получения списка отелей и номеров, что снижает нагрузку на основную БД.
*   **Качество:** Полное покрытие кода unit-тестами (Pytest), использование Ruff для статического анализа и соблюдения стандартов кодирования.
*   **DevOps:** Опыт деплоя на удаленный сервер через Docker Compose, настройка окружения и CI ready структура.



---

### 📫 Связь со мной
*   **Telegram:** [@getattr1](https://t.me/@getattr1)
*   **Email:** [getattr@bk.ru](mailto:getattr@bk.ru)
