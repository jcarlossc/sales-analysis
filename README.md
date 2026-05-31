<div align="center">

# Sales Analysis and Discount Impact

### Pipeline Analítico de Vendas 

Projeto de análise exploratória, estatística e financeira focado na avaliação do impacto dos descontos sobre vendas, faturamento, lucro e margens.

O projeto foi desenvolvido utilizando notebooks Jupyter, modularização em Python, testes automatizados, sistema de logs e configuração centralizada via YAML.

<img src="https://img.shields.io/badge/Python-276DC3?style=for-the-badge&logo=r&logoColor=white" />
<img src="https://img.shields.io/badge/STATUS-EM%20DESENVOLVIMENTO-success?style=for-the-badge" />
<img src="https://img.shields.io/badge/LICENSE-MIT-blue?style=for-the-badge" />
<img src="https://img.shields.io/badge/TESTS-pytest-orange?style=for-the-badge" />

</div>

---

## Objetivos

O projeto busca responder perguntas de negócio como:

* Descontos aumentam vendas, mas reduzem lucro?
* Qual faixa de desconto mantém margens sustentáveis?
* Existem regiões ou categorias mais impactadas?
* Como o desempenho varia ao longo do tempo?
* Quais canais e perfis de clientes geram maior rentabilidade?

## Estrutura do Projeto
```
sales-analysis/
│
├── config/
│   └── config.yaml
├── data/
│   └── sales_data.csv
├── logs/
│   └── sales_analysis.log
├── reports/
│   └── sales_pipeline.html
├── images/
│   ├── sales_01.PNG
│   ├── sales_02.PNG
│   ├── sales_03.PNG
│   ├── sales_04.PNG
│   ├── sales_05.PNG
│   ├── sales_06.PNG
│   ├── sales_07.PNG
│   ├── sales_08.PNG
│   ├── sales_09.PNG
│   ├── sales_10.PNG
│   ├── sales_11.PNG
│   └── sales_12.PNG
│
├── src/
│   └── sales_analysis/
│       ├── dashboard/
│       │     └── dashboard.ipynb
│       ├── graphics/
│       |     ├── graphic_discount_margin.ipynb
│       |     ├── graphic_impact_discount.ipynb
│       |     ├── graphic_months.ipynb
│       │     └── graphic_region_category.ipynb
│       ├── tables/
│       |     ├── table_kpis_list.ipynb
│       │     └── table_progressive_discounts.ipynb
│       ├── utils/
│       │     ├── csv_read/
│       │     │      └── csv_load.ipynb
│       │     ├── loggers/
│       │     │      └── logger.ipynb
│       │     ├── quality/
│       │     │      └── quality_test.ipynb
│       │     └── settings/
│       │            └── quality_test.ipynb
│       │
│       └── sales_pipeline.ipynb
├── .gitignore
├── LICENSE
├── pyproject.toml
├── poetry.lock
└── README.md
```


