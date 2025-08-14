# EDA Lab — MiniLab 01 (Semana 1)

**Objetivo:** EDA do zero para entender distribuição, qualidade e relações das variáveis antes de qualquer modelo.

## Escopo
- Estatística descritiva, missing, outliers (IQR/z-score), correlação.
- ≥3 gráficos (histograma, boxplot, heatmap).
- Entregas: notebook executável, prints, insights e ações.

## Estrutura (projeto)
eda-lab/
├── notebooks
│   └── 01_eda
│       └── 01_minilab01_eda.ipynb
├── docs/                 # imagens/prints p/ README e post
├── data/                 # (gitignored)
├── shiplog/week-01.md
├── journal
|   └── 2025-08-13.md
├── requirements.txt
└── README.md

## Ambiente (Ubuntu 24)
## Preparacao - rodar no Terminal
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
python -m ipykernel install --user --name eda-lab --display-name "Python (eda-lab)"

## Rodar
jupyter lab
# abra: notebooks/01_eda/01_minilab01_eda.ipynb (kernel "Python (eda-lab)")

## Dados
Fonte: sintético (seed=42).
Dicionário: age (num), income (num €/ano), purchases (int), segment (cat A/B/C).

## Saídas (gráficos)
- docs/income_hist.png
- docs/income_box.png
- docs/corr_heatmap.png

## DoD — Semana 1
[ ] Notebook roda fim-a-fim sem erros  
[ ] ≥1 gráfico salvo em docs/ (ideal: 3)  
[ ] 3–5 insights registrados  
[ ] 2–3 ações decididas  
[ ] Tag/commit: w01-v1.0

## Insights (preencher)
1) Método mais rápido do que fazer tabelas dinamicas no excel;  
2) Buscar método para salvar graficos com base no tamanho da base simulada e timestamp da simulacao, gravar csv com a base e gerar arquivo de log. (Tema para o próximo dia).
3) …  
4) …  
5) …

## Ações/Decisões (preencher)
- Decisao em 2025-08-13 > a base sintética é sólida e funciona, vamos mante-lo.
- Decisao em 2025-08-13 > aumentar a base para 50000 e notar a di

## Limitações
Amostra sintética; suposições de normalidade podem não valer em produção.

## Cloud (opcional — GCP Vertex)
gcloud services enable aiplatform.googleapis.com
# Workbench > Managed Notebooks (UI): criar "Python 3 (Data Science)", clonar repo e rodar.

## Custo (semana)
| Prov | Budget € | 25% | 50% | 75% | Gasto |
|------|---------:|:---:|:---:|:---:|------:|
| GCP  | 10       | 🔔  | 🔔  | 🔔  |   0   |

## Reprodutibilidade
pip freeze > requirements.txt  # seed: 42

## Licença
MIT