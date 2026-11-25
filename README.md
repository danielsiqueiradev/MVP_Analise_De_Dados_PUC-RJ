# MVP — Análise de Dados: A Bilheteria do Cinema no Brasil (2009–2017)

MVP da sprint de **Análise de Dados** da pós-graduação em Ciência de Dados e Analytics — **PUC-RJ**.

## Objetivo

Análise exploratória e pré-processamento da bilheteria semanal de cinema no Brasil (2009–2017), respondendo a seis hipóteses (H1–H6) sobre evolução do mercado, participação do cinema nacional, concentração, gêneros e países, sazonalidade e janela de exibição.

## Dataset

**Bilheteria de Obras por Semana** — ANCINE (Dados Abertos do Governo Federal / OCA), obtido em novembro de 2026.

- ~51 mil registros × 15 colunas — um registro = uma obra × uma semana de exibição (qui–qua)
- 3.876 obras únicas (`CPB_ROE`), anos cinematográficos de 2009 a 2017
- O notebook lê o arquivo pela **URL raw deste repositório** (mecanismo oficial de reprodução); `data/` contém a cópia versionada

## Estrutura

```
├── MVP_Bilheteria_Cinema_Brasileiro.ipynb   # notebook/relatório (entregável)
├── data/BilheteriaObrasSemana.csv           # dataset versionado
├── requirements.txt
└── README.md
```

## Como executar

```bash
pip install -r requirements.txt
jupyter notebook MVP_Bilheteria_Cinema_Brasileiro.ipynb
```

**Google Colab:** abrir diretamente em
`https://colab.research.google.com/github/danielsiqueiradev/MVP_Analise_De_Dados_PUC-RJ/blob/main/MVP_Bilheteria_Cinema_Brasileiro.ipynb`
— o dataset é carregado pela URL raw do próprio repositório, sem upload manual.

## Principais achados

- Mercado cresceu **pelo preço**: público +61% vs renda nominal +180% (ingresso médio de R$ 8,61 → R$ 15,00)
- Cinema nacional: **~29% das obras** → **9,6–19,1% do público**, dependente de poucos megassucessos
- Concentração extrema: **10% do catálogo = 80% do público**; top-5 distribuidoras = 70,6%
- Documentário: 14% das obras → **0,4% do público**; animação faz o inverso (6% → ~19%)
- Sazonalidade: julho 1,9x setembro no público semanal médio
- Rendimento por sala **sobe** com a capilaridade — hipótese de saturação **refutada** pelos dados

**Autor:** Daniel Siqueira
