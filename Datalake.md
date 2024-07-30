# Datalake

### Landing Zone

Arquivo raw: synthetic_ecommerce_employee_performance_data.csv

### Stating Zone

Limpeza dos dados: data_quality.ipynb script de limpeza de dados utilizando a biblioteca great-expectations do python, onde o Expectation Results Report informou que todos os dados estão prontos para uso.

### Curated Zone

Dados prontos para análise e construção de relatórios/dashboards: 

- fact_table.csv
- dim_employee.csv
- dim_feedback.csv
- dim_task.csv

### Masked Zone

Aqui é onde é aplicado o mascaramento de dados para proteger informações sensíveis. Nesse caso, a nossa base não possui informação sensível.

### Master Data

É onde ficam os dados principais que são referenciados em diferentes análises. Nesse caso, não possuímos master data.