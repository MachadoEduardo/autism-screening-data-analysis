# Triagem de Autismo em Crianças Pequenas — Análise de Dados

Projeto acadêmico introdutório desenvolvido para praticar conceitos básicos de Ciência de Dados e Introdução à Inteligência Artificial.

O projeto utilizará um conjunto de dados de triagem de autismo em crianças pequenas para explorar etapas como carregamento e leitura de dados, verificação da estrutura do conjunto, tratamento de valores ausentes, análise de tipos, estatística descritiva, identificação de possíveis outliers, visualizações e relações entre variáveis.

> **Aviso:** este projeto possui finalidade exclusivamente acadêmica e educacional. Ele não tem finalidade clínica, não realiza diagnóstico médico e não deve ser utilizado para orientar decisões de saúde.

## Fonte dos dados

O dataset está disponível no Kaggle:

- [Autism Screening for Toddlers](https://www.kaggle.com/datasets/fabdelja/autism-screening-for-toddlers/data)

O notebook baixa o arquivo público automaticamente quando ele ainda não está disponível em `data/raw/`. Os dados locais não são versionados pelo Git. Antes de publicá-los por outro meio, devem ser consultados os termos e a licença apresentados na página do dataset.

## Estrutura do projeto

```text
.
├── data/
│   ├── raw/                 # Dados originais (baixados pelo notebook)
│   └── processed/           # Dados limpos salvos pelo notebook
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

O notebook `01_exploratory_data_analysis.ipynb` já cobre:

- carregamento automático do dataset (quando ainda não estiver em `data/raw/`);
- inspeção da estrutura e verificação de valores ausentes;
- limpeza (nomes de colunas, categorias e duplicatas), ajuste de tipos e salvamento em `data/processed/`;
- **estatística descritiva** de `Age_Mons` e `Qchat-10-Score`, além de contagens de `Class/ASD Traits`, `Sex`, `Jaundice` e `Family_mem_with_ASD`;
- **identificação de possíveis outliers** com boxplot e regra do IQR em `Age_Mons` e `Qchat-10-Score`.

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

- aprofundar visualizações e relações entre variáveis;
- gerar e salvar gráficos em `reports/figures/` quando fizer sentido;
- avaliar futuramente um modelo simples de classificação, sem finalidade diagnóstica.
