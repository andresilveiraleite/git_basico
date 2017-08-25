# Entendendo Merge
## Para unirmos os commits realizados em difentes branchs, podemos utilizar uma funcionalidade muito bacana "O Merge"

Vamos levar em consideração o seguinte cenário: 
2 branchs (master e testes) e 3 commits(C1, C2 e C3) --> sendo que os dois branchs estão apontando para os mesmos commits. 

Vamos criar um novo commit para o branch de testes e outro commit para o branch master. 

Para pegar as alteração que foram realizadas no branch de "testes" e disponibilizar para o branch "master", criaremos um novo commit e nele juntaremos todas as modificações (branch de testes) com os commits existentes no "master".

Visão do cenário:

![Fazendo o Merge](Imagens/merge.jpg)


### Prós:
Operação não destrutiva, ele vai criar um novo commit e juntar tudo. Continuaremos com o histórico intacto.


#### Contras:
É necessário a criação de um novo "Commit", que irá apenas juntar os commits.
O histório fica com muitas informações desnecessárias e de difícil entendimento.

