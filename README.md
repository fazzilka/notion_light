# Notion Light Backend

Pet-проект: упрощённый аналог Notion на FastAPI.  
Фичи:

- Страницы с иерархией (страница внутри страницы)
- Хранение содержимого в JSON (блоки)
- Теги и фильтрация по тегам
- История версий страниц и откат к версии
- Архив (мягкое удаление)
- Публичные ссылки на страницы «только для чтения»
- Docker + Docker Compose
- Alembic миграции, SQLAlchemy 2.x

## Стек

- Python 3.12
- FastAPI
- SQLAlchemy 2.x
- PostgreSQL
- Alembic
- Pydantic v2
- Docker / docker-compose
- GitHub Actions (CI)

Все версии зафиксированы в `requirements.txt`.

---

## Быстрый старт (локально, без Docker)

### 1. Установка

```bash
git clone <url-репозитория> notion-light-backend
cd notion-light-backend

python -m venv .venv
source .venv/bin/activate     # Windows: .venv\Scripts\activate
pip install --upgrade pip
pip install -r requirements.txt
