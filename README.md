# Triagem de Autismo em Crianças Pequenas — Análise de Dados

Projeto acadêmico introdutório desenvolvido para praticar conceitos básicos de Ciência de Dados e Introdução à Inteligência Artificial.

O projeto utilizará um conjunto de dados de triagem de autismo em crianças pequenas para explorar etapas como carregamento e leitura de dados, verificação da estrutura do conjunto, tratamento de valores ausentes, análise de tipos, estatística descritiva, identificação de possíveis outliers, visualizações e relações entre variáveis.

> **Aviso:** este projeto possui finalidade exclusivamente acadêmica e educacional. Ele não tem finalidade clínica, não realiza diagnóstico médico e não deve ser utilizado para orientar decisões de saúde.

## Fonte dos dados

O dataset está disponível no Kaggle:

- [Autism Screening for Toddlers](https://www.kaggle.com/datasets/fabdelja/autism-screening-for-toddlers/data)

O arquivo original deverá ser baixado manualmente e armazenado em `data/raw/`. Antes de publicar os dados no GitHub, devem ser consultados os termos e a licença apresentados na página do dataset.

## Estrutura do projeto

```text
.
├── data/
│   ├── raw/                 # Dados originais, sem alterações
│   └── processed/           # Dados tratados futuramente
├── notebooks/
│   └── 01_exploratory_data_analysis.ipynb
├── src/                     # Funções auxiliares futuras
├── reports/
│   └── figures/             # Gráficos gerados durante a análise
├── .gitignore
├── README.md
└── requirements.txt
```

## Etapa atual

Neste momento, o repositório contém apenas a estrutura inicial do projeto. A análise exploratória e qualquer possível etapa de Machine Learning serão desenvolvidas posteriormente.

## Como preparar o ambiente

Com Python instalado, crie e ative um ambiente virtual e instale as dependências:

```bash
python -m venv .venv
```

No Windows (PowerShell):

```powershell
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
jupyter notebook
```

No Linux ou macOS:

```bash
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

Em seguida, abra o notebook `notebooks/01_exploratory_data_analysis.ipynb`.

## Próximas etapas

- adicionar o dataset original em `data/raw/`;
- documentar e realizar a análise exploratória;
- tratar os dados e, se necessário, salvar uma versão em `data/processed/`;
- gerar e salvar visualizações em `reports/figures/`;
- avaliar futuramente um modelo simples de classificação, sem finalidade diagnóstica.
