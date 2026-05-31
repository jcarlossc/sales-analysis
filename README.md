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

## Tecnologias Utilizadas
| Tecnologias | Descrição |
| ----------- | --------- |
| Python 3.11+ | Linguagem principal |
| Pandas | Biblioteca de Análise de Dados |
| NumPy | Bibliotema Matemática |
| Matplotlib | Biblioteca Gráfica |
| Pytest | Testes | 
| Loguru | Biblioteca de Logs |
| YAML | Serialização de dados |
| Jupyter Notebook | Aplicação web interativa  |
| Poetry | Ferramenta de Gerenciamento |

## Sistema de Logs

O projeto possui logging estruturado com rastreamento completo da execução.

### Exemplo de log
```
2026-05-30T15:49:22.731835-0300 | INFO | Logger configurado com sucesso.
2026-05-30T15:49:28.363737-0300 | INFO | Iniciando leitura do arquivo: C:\workspace\note\sales-analysis\data\sales_data.csv
2026-05-30T15:49:28.687767-0300 | INFO | Arquivo carregado com sucesso. Linhas: 1000 | Colunas: 14
2026-05-30T15:49:29.615446-0300 | INFO | Iniciando testes de qualidade
2026-05-30T15:49:29.816754-0300 | INFO | Métricas básicas concluídas
2026-05-30T15:49:29.862242-0300 | INFO | Teste de qualidade concluída
2026-05-30T15:49:29.863313-0300 | INFO | Finalizando testes de qualidade
2026-05-30T15:49:30.875898-0300 | INFO | Iniciando geração do dashboard
2026-05-30T15:49:30.902859-0300 | INFO | Iniciando cálculos agregados
```

## Testes
Executa testes
```
poetry run pytest --nbmake src/sales_analysis/
```
| Tipo | Está fazendo? | O que valida? |
| ---- | ------------- | --------------|
| Teste de integração |	✅ Sim | Componentes funcionando juntos |
| Teste de execução |	✅ Sim | Notebook roda inteiro |
| Teste smoke/sanity | ✅ Sim | Pipeline não quebra |
| Teste end-to-end | ⚠️ Parcialmente |	Fluxo completo |

O que está sendo validado?
* ✅ imports funcionam
* ✅ YAML carrega
* ✅ logger inicializa
* ✅ DataFrames são criados
* ✅ funções executam
* ✅ gráficos são gerados
* ✅ células executam na ordem
* ✅ dependências estão corretas
* ✅ pipeline completo roda
```
================================================= test session starts =================================================
platform win32 -- Python 3.11.9, pytest-9.0.3, pluggy-1.6.0
rootdir: C:\workspace\note\sales-analysis
configfile: pyproject.toml
plugins: anyio-4.13.0, nbmake-1.5.5
collected 12 items

src\sales_analysis\dashboard\dashboard.ipynb .                                                                   [  8%]
src\sales_analysis\graphics\graphic_discount_margin.ipynb .                                                      [ 16%]
src\sales_analysis\graphics\graphic_impact_discount.ipynb .                                                      [ 25%]
src\sales_analysis\graphics\graphic_months.ipynb .                                                               [ 33%]
src\sales_analysis\graphics\graphic_region_category.ipynb .                                                      [ 41%]
src\sales_analysis\sales_pipeline.ipynb .                                                                        [ 50%]
src\sales_analysis\tables\table_kpis_list.ipynb .                                                                [ 58%]
src\sales_analysis\tables\table_progressive_discounts.ipynb .                                                    [ 66%]
src\sales_analysis\utils\csv_read\csv_load.ipynb .                                                               [ 75%]
src\sales_analysis\utils\loggers\logger.ipynb .                                                                  [ 83%]
src\sales_analysis\utils\quality\quality_test.ipynb .                                                            [ 91%]
src\sales_analysis\utils\settings\setting_yaml.ipynb .                                                           [100%]

Learn more about nbmake at https://github.com/treebeardtech/nbmake

=========================================== 12 passed in 366.97s (0:06:06) ============================================
```

## Licença
Este projeto está licenciado sob MIT License.

## Desenvolvedor focado em:

- Data Engineering
- Analytics
- R Programming
- Python Programming
- Automação de processos
- Engenharia de Software

## Contato
* Autor: Carlos da Costa
* Recife, PE - Brasil
* Telefone: +55 81 99712 9140
* Telegram: @jcarlossc
* Blogger linguagem R: https://informaticus77-r.blogspot.com/
* Blogger linguagem Python: https://informaticus77-python.blogspot.com/
* Email: jcarlossc1977@gmail.com
* LinkedIn: https://www.linkedin.com/in/carlos-da-costa-669252149/
* GitHub: https://github.com/jcarlossc
* Kaggle: https://www.kaggle.com/jcarlossc/
* Twitter/X: https://x.com/jcarlossc1977
