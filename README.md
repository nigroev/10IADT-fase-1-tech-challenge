# 10IADT — Tech Challenge (Fase 1)

Modelo para diagnóstico do câncer de mama. Notebook único: `tech_challenge_fase1.ipynb`.

## Como rodar

### Opção 1 — Docker

```bash
docker build -t tech-challenge-fase1 .
docker run --rm -p 8888:8888 -v "$(pwd):/app" tech-challenge-fase1
```

Acesse `http://localhost:8888` e abra `tech_challenge_fase1.ipynb`.

### Opção 2 — Python local

```bash
python -m venv .venv
source .venv/Scripts/activate     # Linux/Mac: source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```
