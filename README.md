# MVP — Análise de Dados: A Bilheteria do Cinema no Brasil (2009–2017)

MVP da sprint de **Análise de Dados** da pós-graduação em Ciência de Dados e Analytics — **PUC-RJ**.

## Objetivo

Explorar a bilheteria semanal de cinema no Brasil entre 2009 e 2017, respondendo:

1. Como evoluiu o mercado exibidor (público, renda, preço médio, nº de obras)?
2. Qual a participação do cinema nacional no público e na renda?
3. O mercado é concentrado (obras e distribuidoras)?
4. Quais gêneros e países de origem dominam?
5. Existe sazonalidade mensal?
6. Quanto tempo as obras ficam em cartaz e como salas se relacionam com público?

## Dataset

**Bilheteria de Obras por Semana** — ANCINE (Dados Abertos do Governo Federal).

- ~51 mil registros × 15 colunas — um registro = uma obra × uma semana de exibição (qui–qua)
- 3.876 obras únicas (`CPB_ROE`), anos cinematográficos de 2009 a 2017
- Arquivo local: `data/BilheteriaObrasSemana.csv`

## Estrutura

```
├── MVP_Bilheteria_Cinema_Brasileiro.ipynb   # notebook da análise (entregável)
├── data/BilheteriaObrasSemana.csv           # dataset
├── requirements.txt
└── README.md
```

## Como executar

```bash
pip install -r requirements.txt
jupyter notebook MVP_Bilheteria_Cinema_Brasileiro.ipynb
```

O notebook também roda direto no **Google Colab** — basta subir a pasta `data/` ou ajustar o caminho do CSV.

## Principais achados

- O mercado cresceu **pelo preço**: público +61% vs renda nominal +180% (ingresso médio de R$ 8,61 → R$ 15,00)
- Cinema nacional = **~29% das obras** mas apenas **9,6–19,1% do público**, sustentado por poucos megassucessos (*Os Dez Mandamentos*, *Tropa de Elite 2*, *Minha Mãe É uma Peça 2*)
- Concentração extrema: **10% do catálogo = 80% do público**; top-5 distribuidoras (majors) com 70,6%
- Documentário: 14% das obras exibidas para **0,4% do público**; animação faz o inverso (6% → 19%)
- Sazonalidade marcada: julho é o melhor mês (1,9x setembro, o pior)
- Rendimento por sala **sobe** com a capilaridade — blockbuster rende mais por sala, não menos

**Autor:** Daniel Siqueira
