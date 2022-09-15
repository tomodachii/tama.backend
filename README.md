# tama.backend
# backend

- cp .env.template .env
- poetry install
<!-- - docker compose up -d -->
- poetry shell
### Test:

coverage run --source='.' manage.py test --no-input && coverage html && coverage report --skip-covered

### DB Design:

./db.vuerd.json

### Celery:

celery -A main worker -l info -P gevent

### branch naming Convention

https://dev.to/couchcamote/git-branching-name-convention-cch

https://dev.to/i5han3/git-commit-message-convention-that-you-can-follow-1709