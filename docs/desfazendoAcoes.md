# Desfazendo Ações

## Quando realizamos uma alteração e não desejamos continuar com a mesma, podemo desfazé-la

Para realizarmos essa "manobra", podemos utilizar o seguinte comando:

git checkout [nome do arquivo] (ex.: git checkout testes.md)

--> O arquivo alterado irá voltar para sua última versão de "commit".

--> Para confirmarmos, podemos executar o comando "git status" e veremos que não temos mais nenhuma alteração a ser feita.

### E se alterarmos um arquivo e o adicionarmos no git? Não conseguiremos voltar do status "Stage - pronto para commit" para unstage?

Sim, conseguiremos voltar do status "stage" para "unstage".

 Para isso precisamos executar o seguinte comando:

 git reset HEAD [Nome do Arquivo.extensão]  --> Significa que gostaríamos de voltar ao ponto anterior do git (staged --> unstage) 

 Agora, após retornarmos o status, podemos caso seja necessário voltar o arquivo para sua última versão de "commit" (Comando: git checkout [nome do arquivo])

### E se realizarmos um "commit" de uma alteração, conseguiremos voltar o status?

Vamos alterar novamente um arquivo e realizarmos o seguinte comando:

git commit -am "Alterando o arquivo para teste"  --> -a> sigfica incluir todos os arquivos modificados m> Deixar um comentário.

Ou seja, realizamos uma alteração num determinado arquivo, adicionamos o mesmo ao git e executamos o "commit", e agora? Tudo bem, o git possui 3 funcionalidades para resolver esse problema:

1. git reset --soft

O soft retornará o[s] arquivo[s] para o status staged - Ficará Pronto para realização do commit.

2. git reset --mixed

O mixed retornará o[s] arquivo[s] para o status "unstage" - Status pelo qual ainda precisamos incluir as modificações ao git.

3. git reset --hard

O hard simplesmente irá ignorar o que foi alterado nesse commit e voltar ao ponto inicial, como se nada tivesse sido feito.

Observação importante:

Podemos escolher para qual versão gostaríamos de retornar, para isso, utilizaremos a mesma lógica acima, mas passando como parâmetro o identificador de cada commit realizado. Para encontrarmos o identificador de cada commit, precisamos executar o comando:

git log

Logo depois resgatar o identificado anterior ao que gostaria de retornar e executar um dos comandos listados acima de reset:

Exemplo: 

git reset --soft [identicador do commit]
