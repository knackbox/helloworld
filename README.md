# helloworld
Containerised app for testing dev workflows and build pipelines

## Start dev mode

Local build with hot reloads of app changes

```
docker compose up dev --build -d && docker compose logs -f
```

## Start test mode

Local build with actual entrypoint command

```
docker compose up test --build -d && docker compose logs -f
```

## Start prod mode

Pull latest image from ghcr and run actual entrypoint command

```
docker compose up prod -d && docker compose logs -f
```

## Stop

```
docker compose down
```

