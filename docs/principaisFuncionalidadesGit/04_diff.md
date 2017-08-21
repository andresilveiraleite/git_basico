# Visualizando diff

## Antes mesmo de realizar um commit, podemos visualizar quais a alterações foram realizadas.

Para isso, podemos alterar o arquivo que estamos realizando os testes "práticos" com qualquer texto.

Logo depois dessa alteração podemos executar o comando: git diff

Resultado esperado:
- - Altera<E7><E3>o do arquivo criado para validar status do git (modified).

\ No newline at end of file

+ - Altera<E7><E3>o do arquivo criado para validar status do git (modified).

+Alterando arquivo para validar o comando git diff     

>> Vejam que é exibido exatamente o que foi "Adicionado +"

\ No newline at end of file

### Cada mudança que realizarmos, podemos analisar com o "git diff" e com isso teremos a certeza do que foi realizando, antes mesmo de  realizar o "commit".


#### Podemos analisar as diferenças realizadas em vários arquivos com apenas 1 comando:

git diff --name-only    >> Serão exibidos todos os arquivos que foram alterados.