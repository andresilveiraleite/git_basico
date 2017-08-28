# git stash
## Sua função é Guardar as informações que ainda não foram "commitadas" em um local interno do git aonde poderemos resgatar quando quisermos.

### Agora vamos a um exmplo prático:

1. Criar um arquivo em seu repositório.

2. Executar o comando: git status >> Podemos perceber que temos um novo arquivo para ser "commitado".

3. Executar o comando: git stash  >> Vai guardar esse commit para quando quisermos realmente retomá-lo num momento oportuno.

4. Executar novamente o comando: git status >> Podemos perceber que "NÃO" temos o novo arquivo para ser "commitado". O git simplesmente o levou para um local específico para ser manipulado apenas quando quisermos.

5. git stash apply  >> Vai exibir todas as mudanças que havíamos realizado e fazer com que possamos retomá-la.


#### E se tivermos vários arquivos "Ocultados pelo comando git stash", como iremos visualizá-los?

Simples, podemos visualizar todos os "stashs" que temos disponíveis com o seguinte comando:

git stash list



#### E se quisermos apagar todos os "Stashs"?

Para isso, precisamos executar o comando abaixo:

git stash clear


