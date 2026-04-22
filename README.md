# Привет, я Максим 👋
### Python Backend Developer

Специализируюсь на создании асинхронных сервисов и API.

---

### 🛠 Технологический стек

*   **Backend:** Python 3.11+ (FastAPI, Asyncio, Pydantic v2)
*   **Databases:** PostgreSQL (SQLAlchemy ORM, Alembic), Redis
*   **Asynchronous Tasks:** Celery
*   **Infrastructure:** Docker, Docker Compose, Nginx
*   **Testing & Quality:** Pytest, Ruff, MyPy
*   **Tools:** Git, Kibana, Elasticsearch 

---
### 🏗 Мой подход к архитектуре (используется во всех проектах ниже)
Во всех своих проектах я придерживаюсь принципов **Clean Architecture** и разделения ответственности, что делает код тестируемым и поддерживаемым:

*   **Layered Architecture:** Четкое разделение на роутеры (FastAPI), сервисы (Business Logic) и репозитории (Data Access).
*   **Data Integrity:** Использование **DTO (Pydantic v2)** для валидации входящих данных и фильтрации ответов API.
*   **Database Patterns:** Работа с БД через **SQLAlchemy ORM**, управление миграциями через **Alembic**.
*   **Asynchronous:** Подходящее использование `async/await` и вынос тяжелых задач (отчеты, парсинг) в фоновые очереди **Celery + Redis**.
*   **Environment:** Контейнеризация всего окружения через **Docker Compose** для быстрого развертывани
