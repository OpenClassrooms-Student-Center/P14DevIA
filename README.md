# NewsFoundry

## Prérequis

- Docker
- Python 3.13
- uv
- Node.js 22.19

## Installation

1. Cloner le repository
2. Démarrer le backend aved les instructions du fichier `backend/README.md`
3. Initialiser un projet Next.js dans un dossier `frontend/`


## Stack technologique

### Frontend

**Next.js**

### Backend

- **Python** pour bénéficier de son écosystème de librairies IA
- **FastAPI** pour le développement de l'API
- **SQLModel** en ORM branché à une base de données postgres
- **PydanticAI** comme client LLM
- **LlamaIndex** pour la RAG
- **WorldNewsAPI** comme source d'actualités

### Deploiement

#### Frontend

Déployer le frontend sur [Vercel](https://vercel.com/dashboard).

#### Backend

Déployer le backend sur [Railway](https://railway.com/dashboard).

> Un Dockerfile est déjà présent pour faciliter le déploiement. Il faudra simplement référencer `backend/` comme "Root Directory" après avoir connecté le repository.
> La base de donnée postgres peut être créée via Railway dans le même projet que le backend.