# Banco1

```
 -- Aula 25/09/24
 -- Exercícios SQL
 -- GABRIEL SANDES
```

```sql
 -- criar tabela Clientes1
 create table Clientes1(
 id_cliente int primary key,
 nome_cliente varchar (100),
 email_cliente varchar (150),
 data_nascimento date,
 telefone_cliente varchar (15)
 );
 
```

```sql
 -- criar tabela Produtos1 
 create table Produtos1(
 id_produto int primary key,
 nome_produto varchar (100),
 preco_produto decimal (8,2)
 );
 

```

```sql

 -- criar tabela Faturas1
 create table Faturas1(
 id_fatura int primary key,
 data_criacao date,
 valor_fatura decimal(10,2)
 );

```
 
 