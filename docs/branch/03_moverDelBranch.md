# Mover e Deletar Branch
## Podemos realizar a movimentação ou até mesmo a exclusão de branchs com muita facilidade

Primeiramente vamos validar quais o branchs existentes com o comando:

git branch

Agora vamos mudar do branch que estamos para outro existente:

git checkout testes  >> Basta logo após o comando de checkout, preenchermos com o branch desejado.

### Para excluírmos um branch que não iremos mais utilizar, devemos utilizar o comando abaixo:

git branch -D testes

Para validarmos se o branch realmente foi excluído com sucesso, devemos executar o comando abaixo:

git branch
 

