## Visões Finais dos Dados

### Visão 1: Desempenho por funcionário

```sql
SELECT e.EmployeeName, e.Department, 
       SUM(f.Duration) AS TotalDuration,
       SUM(f.OrdersProcessed) AS TotalOrdersProcessed, 
       SUM(f.ComplaintsHandled) AS TotalComplaintsHandled
FROM fact_table f
JOIN dim_employee e ON f.EmployeeID = e.EmployeeID
GROUP BY e.EmployeeName, e.Department
```

Esta visão foca no desempenho individual de cada funcionário, permitindo a análise de eficiência e produtividade por pessoa. Com essa tabela é possível fazer o monitoramento de produtividade, identificação de necessidades de treinamento e reconhecer funcionários de alto desempenho. 

### Visão 2: Análise de tarefas e feedback

```sql
SELECT t.TaskType, 
       AVG(f.Duration) AS AvgDuration, 
       SUM(f.OrdersProcessed) AS TotalOrdersProcessed, 
       SUM(f.ComplaintsHandled) AS TotalComplaintsHandled, 
       fb.Feedback, 
       COUNT(*) AS FeedbackCount
FROM fact_table f
JOIN dim_task t ON f.TaskTypeID = t.TaskTypeID
JOIN dim_feedback fb ON f.FeedbackID = fb.FeedbackID
GROUP BY t.TaskType, fb.Feedback
```

Esta visão analisa o desempenho baseado nos tipos de tarefa e no feedback recebido, fornecendo insights sobre quais tarefas são mais eficientes e quais áreas podem precisar de melhorias. Com essa tabela é possível identificar quais tipos de tarefas estão levando mais tempo e podem ser otimizadas, identificar áreas que precisam de melhorias e alocar recursos humanos e financeiros.