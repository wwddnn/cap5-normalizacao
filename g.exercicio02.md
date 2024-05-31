## exercicio 02
normalize a seguinte relação, aplicando as 3 formas normais:

```
Pedido(nro-pedido, data, nro-peca, descricao, qtd_comprada, preco_comprado)

* nro-pedido é chave primária.

* nro-peça é chave primária. 
```


## resolução do exercício
obs. é sempre indicado fazer também a representação das intâncias, que são as tabelas mesmo em si, para ter uma visão melhor do problema.

* para escrevermos a relação textual abaixo, temos que ver a tabela, e começamos pelas tabelas que não tem relação estrangeira.

```
Pedido(nro-pedido, data)

* nro-pedido é chave primária.

* data é o atributo dependente.

```


```
Peca(nro-peca, descricao)

* nro-peca é chave primária.

* descrição é o atributo dependente.
```


```
Pedido_peca(nro-pedido, nro-peca, qtd_comprada, preco_cotado)
    nro-pedido referencia Pedido
    nro-peca referencia Peca

* nro-pedido é chave primária.

* nro-peca é chave primária.

* qtd_comprada e preco_cotado são atributos dependentes.

* essa tabela, ou seja essa relação vai representar tanto o pedido quanto a peça.
```

