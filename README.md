# Migrations Alembic

À initialiser avec :

```bash
alembic init database/migrations
```

Puis configurer `sqlalchemy.url` dans `alembic.ini` pour pointer vers
`config.settings.settings.database_url`, et importer `database.base.Base`
ainsi que tous les modèles dans `env.py` afin qu'Alembic détecte le schéma
cible (`target_metadata = Base.metadata`).
