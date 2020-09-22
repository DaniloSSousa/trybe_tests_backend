## Exercícios de queries do mongodb

1: Utilizando o estágio $match, escreva uma agregação para retornar somente os clientes do sexo "MASCULINO".

2: Utilizando o estágio $match, escreva uma agregação para retornar somente os clientes do sexo "FEMININO" e com data de nascimento entre os anos de 1995 e 2005.

3: Utilizando o estágio $match, escreva uma agregação para retornar somente os clientes do sexo "FEMININO" e com data de nascimento entre os anos de 1995 e 2005, limitando a quantidade de documentos retornados em 5.

4: Conte quantos clientes do estado SC existem na coleção. Retorne um documento em que o campo _id contenha a UF e outro campo com o total.

5: Agrupe os clientes por sexo. Retorne o total de clientes de cada sexo no campo total.

6: Agrupe os clientes por sexo e uf. Retorne o total de clientes de cada sexo no campo total.

7: Utilizando a mesma agregação do exercício anterior, adicione um estágio de projeção para modificar os documentos de saída, de forma que se pareçam com o documento abaixo (não se importe com a ordem dos campos):
```
{
  "estado": "SP",
  "sexo": "MASCULINO",
  "total": 100
}
```

8: Descubra quais são os 5 clientes que gastaram o maior valor.

9: Descubra quais são os 10 clientes que gastaram o maior valor no ano de 2019.

10: Descubra quantos clientes compraram mais de 5 vezes. Retorne um documento que contenha somente o campo clientes com o total de clientes.
Dica: O operador $count pode simplificar sua query.

11: Descubra quantos clientes compraram menos de três vezes entre os meses de Janeiro de 2020 e Março de 2020.

12: Descubra qual as três ufs que mais compraram no ano de 2020. Retorne os documentos no seguinte formato:
```
{
  "totalVendas": 10,
  "uf": "SP"
}
```

13: Encontre qual foi o total de vendas e a média de vendas de cada uf no ano de 2019. Ordene os resultados pelo nome da uf. Retorne os documentos no seguinte formato:
```
{
  "_id": "MG",
  "mediaVendas": 9407.129225352113,
  "totalVendas": 142
}
```
