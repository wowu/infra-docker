# BIT Infra - Docker (2021-12-09)

Wprowadzenie do Dockera.

## Zadania

### 1. Hello world!

```bash
docker run --rm hello-world
```

### 2. Flask

- Utwórz `Dockerfile` dla przykładowej aplikacji
- Utwórz `docker-compose.yml` uruchamiający aplikację z volume zamontowanym w `/app/db` i z wystawionym portem.

```bash
docker build -t flask .

docker run --rm -p 80:3000 flask
docker run --rm -p 80:3000 -v $(pwd)/db:/app/db -p 80:3000 flask

docker-compose up
```
