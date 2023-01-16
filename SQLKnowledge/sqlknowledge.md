# SQL Server query execution order. Would like to understand how SQL Server executes a query. There are at least

- Query Parsing
  - **Parser**: Query syntax parses and validates then it will convert to an execution tree
  - **Algebrizer**: The execution engine needs to verify all objects such as columns, table names etc.  
- Query Compilation
  - **Compilation:** The Query tree is complied by the optimizer if it is executing the first time otherwise SQL server uses the existing compiled query plan.
- Query Optimization
  - **Optimization**: The query optimizer considers optimizing some operators such as joins, select etc.
  