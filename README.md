# ml-serving

model serving: fastapi inference, training pipeline, react dashboard, infra

## architecture

- **`inference/`** — fastapi inference api
- **`training/`** — pandas/numpy training pipeline
- **`dashboard/`** — react metrics dashboard
- **`infra/`** — terraform + gpu nodepool

Each service is independently buildable; `docker-compose.yml` wires them
together for local dev.

## running locally

```
docker compose up --build
```

## layout

```
ml-serving/
  inference/
  training/
  dashboard/
  infra/
  docker-compose.yml
  Makefile
```

