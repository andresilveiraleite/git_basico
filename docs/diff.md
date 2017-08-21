# Visualizando diff

## Antes mesmo de realizar um commit, podemos visualizar quais a alterações foram realizadas.

Para isso, podemos alterar o arquivo que estamos realizando os testes "práticos" com qualquer texto.

Logo depois dessa alteração podedmos executar o comando: git diff

Resultado esperado:
diff --git a/novoArquivoGit.md b/novoArquivoGit.md

index 48b6e6e..62de31e 100644

--- a/novoArquivoGit.md

+++ b/novoArquivoGit.md

@@ -1,2 +1,3 @@

 TESTE
 
- - Altera<E7><E3>o do arquivo criado para validar status do git (modified).

\ No newline at end of file

+ - Altera<E7><E3>o do arquivo criado para validar status do git (modified).

+Alterando arquivo para validar o comando git diff     

>> Vejam que é exibido exatamente o que foi "Adicionado +"

\ No newline at end of file

Cada mudança que fizermos, podemos analisar com o "git diff" e analisar ser realmente o que iremos realizar o "commit", tudo está de acordo com o que esperamos.

### Podemos analisar as diferenças realizadas em vários arquivos com apenas 1 comando:

git diff --name-only   >> Serão exibidos todos os arquivos que foram alterados.