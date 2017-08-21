# Enviando mudanças do repositório Local para o Remoto
## Após efetuarmos mudanças no repositório local, precisamos enviá-las para o remoto

Para isso, precisaremos alterar qualquer arquivo em nosso repositório local.

Executar o comando para análise da mudança: git status.

Realizar o commit dessa alteração: git commit -am "Enviar mudanças do local para o remoto - github"

Executar o comando para análise do log: git log

Podemos perceber que já temos essa alteração no nosso repositório local, mas caso fóssemos procurá-lo no github, ele ainda não existiria, pois ainda não o enviamos.

Para enviarmos essa mudança local para o remoto, devemos utilizar o seguinte comando:

git push origin   --> Para onde quero enviar: origin (repositório remoto - nome padrão) e o branch que estou "master"

A partir desse momento, todas as alterações realizadas localmente serão enviadas "atualizadas" no repositório remoto.


