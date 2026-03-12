# Comandi Codinator

## Primo avvio
```bash
cd /workspaces/WebAppClaude/codinator
docker compose up --build -d
```

## Avvio normale
```bash
docker compose up -d
```


## Reset completo in caso di malfunzionamento (cancella il DB)
```bash
docker compose down
docker volume rm codinator_db_data
docker compose up --build -d
```

## Porte
| Porta | Servizio |
|-------|----------|
| `8080` | App |
| `8081` | phpMyAdmin |
