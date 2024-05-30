## 2FN
uma relação esta na 2FN quando duas condições são satisfeitas:

1. a relação esta na 1FN.

2. todos os atributos que não forem chave primária, dependem funcionalmente de toda a chave primária.

* não pode haver dependência parcial. ou seja um atributo tem que depender de toda a chave primária.



o que fazer?

1. identificar todos os atributos que não possuem dependência total da chave.

2. remover os atributos nessa situação ou então criar novas relações de forma a não haver dependências parciais. 

* a ideia é não ter mais dependências parciais.




exemplo: 

- tabela empregado:

Empregado(CPF, nome)

*CPF é chave primária.

* os elementos não se repetem


- tabela Projeto:

Projeto(codProj, nome, local)

* codProj é chave primária

* os elementos não se repetem


- tabela Empregado_projeto:

Empregado_projeto(CPF, codProj, horasTrabalho)

* CPF e cof_proj são chaves primárias dessa tabela resultante, mas são chave estrangeira da tabela Empregado(cpf) e da tabela Projeto(codProj).

* é uma tabela resultante aqui, os elementos podem se repetir


obs. antes era uma tabela só, contemplando tudo, agora são 3 tabelas, ou seja uma tabela para Empregados, uma tabela para Projeto, e outra tabela Empregado_projeto.