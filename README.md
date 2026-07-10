# analise-vendas-jogos-2d-vs-3d
# 2D vs 3D: qual estilo de jogo vende mais?

A ideia desse projeto surgiu de uma pergunta simples que qualquer estúdio de jogos precisa responder na hora de decidir onde investir: vale mais a pena apostar em jogos 2D ou 3D?

## O que eu queria descobrir

Duas coisas, principalmente:

- Jogos 3D realmente vendem mais que jogos 2D?
- Isso muda dependendo de quem está jogando? Um jogo pra criança segue o mesmo padrão de um jogo pra adulto?

## O que eu encontrei

Jogos 3D vendem, em média, cerca de **17% a mais** que jogos 2D, e isso é estatisticamente significativo (testei com Mann-Whitney U, p = 0,000008). Testei também se essa vantagem mudava por faixa etária e a resposta foi não: o 3D vende mais em praticamente todos os públicos, de forma bem consistente.

A parte mais interessante veio quando olhei pro público infantil especificamente. Ali o cenário se inverte: **66% dos jogos voltados pra crianças são 2D**, contra só 32% nos demais públicos. Ou seja, mesmo o 3D vendendo mais no geral, o 2D continua sendo a escolha natural quando o jogo é pra criança.

## Como cheguei nesses números

1. Limpeza e tratamento dos dados
2. Análise exploratória pra entender a distribuição dos dados antes de qualquer teste
3. Três testes de hipótese: Mann-Whitney U, ANOVA de duas vias e teste Z de proporções
4. Cálculo de alguns indicadores de negócio (participação de mercado, ticket médio por região etc.)
5. Um dashboard no Tableau pra visualizar tudo de forma mais direta

## O que tem nesse repositório

```
├── notebook/         -> o caderno Jupyter com toda a análise, do começo ao fim
├── apresentacao/      -> slides resumindo os principais achados
└── imagens/           -> print do dashboard
```

## Ferramentas

Python (pandas, numpy, scipy, statsmodels, matplotlib, seaborn) pra análise, e Tableau Public pro dashboard interativo.

## Dashboard

Dá pra explorar os dados de forma interativa aqui: [Tableau Public](https://public.tableau.com/app/profile/raphael.victor/viz/Analise_Vendas_Jogos_2D_3D/Jogos2Dvs3DAnlisedeVendas)

![Dashboard - Análise de Vendas de Jogos 2D vs 3D](imagens/dashboard.png)

---

Raphael Victor
[LinkedIn](#) · [GitHub](https://github.com/Rapha77y)

*Nota técnica: dataset simulado, construído para fins de estudo do processo analítico.*
