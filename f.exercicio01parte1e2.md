## exercicio 01 parte 1 e 2

procurar aplicar as três formas normais, na ordem, e entender o conceito de dependência funcional, e também de dependência transitória.

ao aplicar as três normas, a tabela resultante será:

```
Aluno (cod_aluno, nome_aluno, cod_local_nasc)

* cod_aluno é chave primária
```


```
Local (cod_local, cidade, UF)

*cod_local é chave primária

* essa tabela esta conectada a tabela Aluno através da chave estrangeira cod_local.
```


```
Disciplina (cod_disciplina, nome_disciplina)

* cod_disciplina é chave primária

* essa tabela esta conectada a tabela Matricula através da chave primária cod_disciplina
```


```
Matricula (cod_aluno, cod_local, cod_disciplina)

* cod_aluno, cod_local e cod__disciplina são chave estrangeira para as tabelas Aluno, Local e Disciplina.

* essa é uma tabela resultante das outras.
```



## fazendo a representação textual do exercício anterior
começar com as representações que não tem chave estrangeira. nesse caso são as tabelas Local, e a tabela Disciplina. fica assim:

```
Local(cod_local, cidade, UF) 

* cod_local é chave primária.
```

```
Disciplina (cod_disciplina, nome_disciplina) 

* cod_disciplina é chave primária.
```


agora vamos fazer da tabela Aluno:

```
Aluno(cod_aluno, nome_aluno, cod_local_nasc)
    cod_local_nasc referencia Local

* onde cod_aluno é chave primária, e cod_local_nasc é chave estrangeira que faz referencia a tabela Local no campo cod_local.

* dica: colocar a chave estrangeira, nesse caso cod_local_nasc e sua referencia com uma margem de tab e também na linha abaixo. alguns autores gostam de colocar também na cor vermelha.
```

agora vamos fazer a tabela Matricula:

```
Matricula(cod_aluno, cod_turma, cod_disciplina)
    cod_aluno referencia Aluno
    cod_disciplina referencia Disciplina

 * temos nessa tabela uma chave primária composta, por cod_aluno e por cod_turma.
```







