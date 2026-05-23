# 10IADT — Tech Challenge (Fase 1)

Sistema de suporte ao diagnóstico do câncer de mama. Notebook único: `tech_challenge_fase1.ipynb`.

## Como rodar

### Opção 2 — Python local

```bash
python -m venv .venv
source .venv/Scripts/activate     # Linux/Mac: source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

## Executar o notebook end-to-end (gerar outputs)

```bash
docker run --rm -v "$(pwd):/app" -w /app tech-challenge-fase1 \
    jupyter nbconvert --to notebook --execute tech_challenge_fase1.ipynb \
    --inplace --ExecutePreprocessor.timeout=1200
```
