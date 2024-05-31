## exercício 03
normalize a seguinte relação:
```
Cliente(nro-cli, nome, end_entrega)

* nro-cliente é chave primária.
```



## resolução do exercício

```
Cliente(nro-cliente, nome)

* nro-cli é chave primária.
```

```
Cliente-entrega(nro-cli, end_entrega)
    nro-cli referencia Cliente

* nro-cli e end_entrega são chaves primárias compostas.
```



