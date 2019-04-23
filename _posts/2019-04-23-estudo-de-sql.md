# Estudando sql

## Criando a estrutura 
Para criarmos um banco de dados funcional, precisamos dizer isso ao banco de dados:


```sql
create database nome;
use nome;
```

Em nosso caso vamos chamar de **petshop**. 

## Criando as tabelas
Para criarmos um banco, devemos criar as tabelas, para isso:

```sql
create table nome(
    id tipo chave primaria,
    coluna tipo,
    coluna tipo,
    coluna tipo
);
```

Em nosso caso vamos criar as seguintes tabelas com os seguintes tipos:








# Criando funções com *plsql*





```sql
create type type_aniversario_pessoa as();

```



```sql
create or replace function mandar_cartas(integer)
    returns setof type_aniversario_pessoa
as $$
declare
    dados_aniversario type_aniversario_pessoa
begin
    update pessoas set carta = TRUE where extracr(Month )
end
$$ LANGUAGE 'plsql';
```