# FastAPI - Docker - Test Driven Development

![Continuous Integration and Delivery](https://github.com/antoniovmonge/fastapi-tdd/workflows/Continuous%20Integration%20and%20Delivery/badge.svg?branch=main)

```bash
uvicorn app.main:app --reload
```

Apply migrations

```bash
docker-compose exec web aerich upgrade
```

Run Tests

```bash
docker-compose exec web python -m pytest -p no:warnings
```

Run tests with coverage

```bash
docker-compose exec web python -m pytest -p no:warnings --cov="."
```

Run Flake8

```bash
docker-compose exec web flake8 .
```
