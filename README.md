# Análise de Crescimento da Telemedicina

Este repositório contém o notebook `analise_crescimento_telemedicina_P2.ipynb`, que desenvolve uma análise exploratória de dados (EDA) e um modelo supervisionado para identificar padrões de alto crescimento no uso de telemedicina entre diferentes combinações de estado, trimestre e perfis demográficos.

## Integrantes

- Gabriel Mediotti Marques – RM 552632
- Jo Sales – RM 552679
- Miguel Garcez de Carvalho – RM 553768
- Vinicius Souza e Silva – RM 552781


## Conteúdo

- `analise_crescimento_telemedicina_P2.ipynb`: notebook principal com todo o fluxo da análise.
- `TMEDTREND_PUBLIC_250827.csv`: base pública do Medicare utilizada na investigação.

## Fluxo Analítico

1. Carregamento e inspeção do dataset.
2. Limpeza e filtragem de registros para garantir comparações válidas entre trimestres.
3. Criação das variáveis de crescimento (`Delta_Telehealth`, `Prev_Pct_Telehealth` e `HighGrowth`).
4. EDA com foco em entender padrões de adoção por ano, faixa etária, raça e ruralidade.
5. Construção de um pipeline com pré-processamento (One-Hot Encoding, padronização) e modelo `RandomForestClassifier` para prever `HighGrowth`.
6. Avaliação via métricas de classificação (precisão, recall, F1, ROC-AUC) e análise de importância das features.

## Requisitos

- Python 3.10+
- Bibliotecas principais: `pandas`, `numpy`, `matplotlib`, `scikit-learn`

Instale as dependências com:

```bash
pip install -r requirements.txt  # ou instale manualmente as bibliotecas listadas acima
```

## Como executar

1. Coloque o arquivo `TMEDTREND_PUBLIC_250827.csv` na mesma pasta do notebook.
2. Abra `analise_crescimento_telemedicina_P2.ipynb` em um ambiente compatível (VS Code, JupyterLab, etc.).
3. Execute as células na ordem apresentada para reproduzir a análise completa.