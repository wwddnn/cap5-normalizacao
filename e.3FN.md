## 3FN
é o último nível de análise que vamos fazer.

se a relação estiver na 3FN, dissemos que essa relação já esta normalizada.



uma relação esta na 3FN quando duas condições estão satisfeitas:
1. a relação esta na 2FN.

2. não exitem atributos não chave que sejam dependentes de outros atributos não chave.

3. atributos não chave devem depender exclusivamente de atributos chave.

* dependência transitiva é quando um atributo não chave dependem de um outro atributo não chave. 

* a ideia aqui nessa 3FN é evitar a dependência transitiva.

* a ideia é que um atributo não chave deve depender de um atributo chave.





como colocar uma relação na 3FN :

1. identificar todos os atributos que são funcionalmente dependentes de outros atributos não chave. (ou seja identificar as dependências transitivas).

2. remover os atributos com dependência transitiva ou separar as relações. ( ou seja vejo se o atributo não chave é importante, caso não seja importante então excluo ele, mas se for importante então vou separar as relações).

