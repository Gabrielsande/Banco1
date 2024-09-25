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

```
 -- EXERCÍCIOS DAS 20 PERGUNTAS
```



```sql

 -- criar tabela Faturas1
 create table Faturas1(
 id_fatura int primary key,
 data_criacao date,
 valor_fatura decimal(10,2)
 );

```
 
```sql 
-- criar tabela Funcionarios
create table Funcionarios(
id_funcionario int primary key,
nome_funcionario varchar(30),
sobrenome_funcionario varchar(30),
salario_funcionario decimal(10,2) 
);

alter table Funcionarios add Data_Nascimento date;
alter table Funcionarios rename column sobrenome_funcionario to apelido_funcionario;
alter table Funcionarios add id_endereco int;
```

 ```sql

alter table Funcionarios add IDDepartamento int;

-- criar tabela Projetos
create table Projetos(
id_Projeto int primary key,
nomeProjeto varchar(50)
);

alter table Projetos add IDCliente int;

```

```sql
-- criar tabela Alocacoes
create table Alocacoes(
id_alocacoes int primary key,
id_funcionario int,
id_Projeto int
);

```
```sql
-- criar tabela Cliente2
create table Cliente2(
id_cliente2 int primary key,
nome_cliente varchar(50)
);

alter table Cliente2 rename column nome_cliente to NomeEmpresa;

```

```sql
-- criar tabela Endereco
create table Endereco(
id_endereco int primary key,
rua_endereco varchar(100),
cidade_endereco varchar(100),
cep_endereco int(50)
);
```
```sql
-- criar tabela Pedidos
create table Pedidos(
id_pedidos int primary key,
data_pedidos date
);

alter table Pedidos add id_cliente2 int;

```
```sql
-- criar tabela ItensPedidos
create table itensPedidos(
id_itensPedidos int primary key,
id_pedido int,
id_produto int
);
```
```sql
-- criar tabela estoques
create table Estoques(
id_estoques int primary key,
quantidade_estoques int
);

alter table Estoques add id_produto int;
```
```sql
-- criar tabela vendas
create table vendas(
id_vendas int primary key,
dataVenda date
);

alter table vendas add id_cliente2 int;
```