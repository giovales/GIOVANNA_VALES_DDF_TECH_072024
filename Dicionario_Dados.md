# Dicionário de Dados

**Nome do Dataset:** synthetic_ecommerce_employee_performance_data.csv

**Descrição:** Conjunto de dados sintético contendo informações sobre as tarefas realizadas por funcionários de e-commerce, incluindo tipo de tarefa, duração, número de pedidos processados, reclamações respondidas, feedback dos clientes e tempo de resposta.

**Fonte:** Código de geração da base sintética disponível no [GitHub](https://github.com/giovales/GIOVANNA_VALES_DDF_TECH_072024/blob/main/data/dataset.ipynb).

**Frequência de Atualização:** Conjunto de dados histórico, não atualizado.

**Última Atualização:** 25/07/2024

**Tags:** E-commerce, Desempenho de Funcionários, Case Técnico.

**Dicionário de Dados**

Abaixo estão os detalhes de cada coluna no conjunto de dados sintético de desempenho de funcionários de e-commerce.

**Detalhes dos Campos**

- **EmployeeID**
    - **Tipo de Dado:** String
    - **Exemplo:** d290f1ee-6c54-4b01-90e6-d701748f0851
    - **Descrição:** Identificador único do funcionário, usado para diferenciar e agrupar as atividades realizadas por cada funcionário.
- **TaskDate**
    - **Tipo de Dado:** Data
    - **Exemplo:** 2023-07-25
    - **Descrição:** Data em que a tarefa foi realizada, usada para análise temporal das atividades.
- **TaskTime**
    - **Tipo de Dado:** Hora
    - **Exemplo:** 14:30:00
    - **Descrição:** Hora em que a tarefa foi iniciada, útil para analisar a distribuição das atividades ao longo do dia.
- **TaskType**
    - **Tipo de Dado:** String
    - **Exemplo:** customer_service
    - **Descrição:** Tipo de tarefa realizada, categorizando as atividades para análise de carga de trabalho e eficiência. Valores possíveis: 'customer_service', 'order_processing', 'inventory_management'.
- **Duration**
    - **Tipo de Dado:** Inteiro
    - **Exemplo:** 45
    - **Descrição:** Duração da tarefa em minutos, usada para avaliar a eficiência e o tempo gasto em cada tipo de atividade.
- **OrdersProcessed**
    - **Tipo de Dado:** Inteiro
    - **Exemplo:** 30
    - **Descrição:** Número de pedidos processados durante a tarefa, importante para medir a produtividade do funcionário.
- **ComplaintsHandled**
    - **Tipo de Dado:** Inteiro
    - **Exemplo:** 5
    - **Descrição:** Número de reclamações atendidas durante a tarefa, usado para avaliar a capacidade de resolução de problemas.
- **Feedback**
    - **Tipo de Dado:** String
    - **Exemplo:** positive
    - **Descrição:** Feedback dos clientes sobre a tarefa realizada, usado para medir a satisfação do cliente e identificar áreas de melhoria. Valores possíveis: 'positive', 'negative', 'neutral'.
- **ResponseTime**
    - **Tipo de Dado:** Inteiro
    - **Exemplo:** 10
    - **Descrição:** Tempo de resposta a solicitações em minutos, importante para avaliar a velocidade do atendimento ao cliente.