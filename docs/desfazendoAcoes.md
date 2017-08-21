# Desfazendo Ações

## Quando realizamos uma alteração e não desejamos continuar com a mesma, podemo desfazé-la

Para realizarmos essa "manobra", podemos utilizar o seguinte comando:

git checkout [nome do arquivo] (ex.: git checkout testes.md)

--> O arquivo alterado irá voltar para sua última versão de "commit".

--> Para confirmarmos, podemos executar o comando "git status" e veremos que não temos mais nenhuma alteração a ser feita.

### E se alterarmos um arquivo e o adicionarmos no git? Não conseguiremos voltar do status "Stage - pronto para commit" para unstage?

Nesse caso, teremos que alterar um arquivo e adicioná-lo ao git (git add *) e logo em seguida para constatarmos a ação, devemos realizando o seguinte comando "git diff", não iremos encontrar nenhuma diferença pois esse arquivo está pronto para realizarmos o "commit".

 Agora iremos responder a pergunta do tópico \o/, sim conseguiremos voltar do status "stage" para "unstage".

 Para isso precisamos executar o seguinte comando:

 git reset HEAD [Nome do Arquivo.extensão]  --> Significa que gostaríamos de voltar ao ponto anterior do git (stage --> unstage) 

 Agora, após retornarmos o status, podermos caso seja necessário voltar o arquivo para sua última versão de "commit" (Comando: git checkout [nome do arquivo])


