# NewsFoundry Backend

1. Copier le fichier `.env.example` dans `.env`


2. Installer les dépendances:
```bash
uv sync
```

2. Démarrer la base de données:
```bash
docker run \
  --name newsfoundry_db \
  -e POSTGRES_USER=user \
  -e POSTGRES_PASSWORD=password \
  -e POSTGRES_DB=newsfoundry \
  -p 5432:5432 \
  postgres:17
```

3. Lancer le backend:
```bash
uv run --env-file .env src/main.py
```

## Deploiement

Déployer le backend sur [Railway](https://railway.com/dashboard).
Un dockerfile est déjà présent pour faciliter le déploiement. Il faudra simplement référencer `backend/` comme "Root Directory" après avoir connecté le repository.

La base de donnée postgres peut être créée via Railway dans le même projet que le backend.