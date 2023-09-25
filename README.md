# Atividade_SQLAdelson

1. Selecione todos os dados dos países da tabela_paises;
 
![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/3e95dd45-0960-4e02-98e8-437b3ad9696d)

## Resultado esperado

![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/4fbff040-80b2-4090-b332-08367235143e)

2. Selecione todas as cidades cujo país seja brazil;

![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/43fdda5f-2cfc-4154-b94f-4eaff2e48f1a)

## Resultado esperado

![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/0e9af085-3e68-4cfb-9a88-b12ce31ba661)

3. Selecione todas as cidades cuja região(estado) é ceará;

select cidade from tabela_paises where regiao = 'Ceará';

## Resultado esperado

![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/5f8ad4af-0a9d-4daa-8ae9-84ab74b04a7c)


4. Utilize a função count para saber quantas regiões(estados) existem na China,
utilize também o group by;

select count(*) as quantidade_regioes from tabela_paises where pais = 'China' group by regiao;

## Resultado esperado

![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/8d09302b-a3ed-4c34-8c15-17df6fcdedf1)

5. Quais regiões, diferentes, existem no Canadá?

select distinct regiao, count(*) as quantidade_regioes from tabela_paises where pais = 'Canada' group by regiao;

## Resultado esperado

![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/65eac936-fa57-4167-9ef9-6358a8e9f041)

6. Quantos países diferentes existem na tabela 'tabela_paises';

select count(distinct pais) as paises_distintos from tabela_paises;

## Resultado esperado

![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/ab41a13d-3247-4411-92a7-00884108e850)

7. Quantas cidades diferentes existem no brazil;

select count(distinct cidade) as cidades_diferentes from tabela_paises where pais = 'Brazil';

## Resultado esperado

![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/62c5d451-4d81-4f24-ae88-9d455e6ea291)

8. Selecione os países e quantas regiões cada país possui;

select pais, count(distinct regiao) as quantidade_regioes from tabela_paises group by pais;

## Resultado esperado

![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/28dc1a6c-fa01-4a7e-9929-d062460c54aa)

9. Quantas pessoas com nome começando em 'João' existem no banco?

select count(*) as quantidade_pessoas from tabela_paises where nome like 'João%';

## Resultado esperado

![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/d409e80c-4743-4c28-a53f-d3894a522289)

10. Quantas pessoas têm o nome John?

select count(*) as quantidade_john from tabela_paises where nome like  'John%';

## Resultado esperado

![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/6eb27016-6b0e-45e4-ad67-430443578cdb)

11. Ordene os nomes dos países sem repetição em ordem alfabética;

select distinct pais from tabela_paises order by pais;

## Resultado esperado

![image](https://github.com/Ksuz/Atividade_SQLAdelson/assets/117034772/ffa6b696-9ca1-4178-ab31-500199b5e30a)

