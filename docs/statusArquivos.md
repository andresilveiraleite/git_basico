# O Ciclo de vida dos status dos Arquivos

## O git separa em 4 estados bem definidos como os arquivos serão "Operacionalizados":

1. Untacked
O momento em que o arquivo acabou de ser adicionado no repositório e o git ainda não conhece nenhuma versão desse arquivo.

2. Unmodified
O momento que o arquivo é adicionado ao git.

3. Modified
O momento em que "modificamos" um determinado arquivo que foi adicionado.

4. Staged
O momento em que o arquivo está pronto para ser "Versionado". 

Assim que realizarmos o "Commit - Criaremos uma nova versão", os arquivos irão retornar para o status "Unmodified".

### Analisando qual o nosso diretório e o status inicial do GIT:

1. Validar diretório atual:

    Devemos iniciar o programa "GIT-BASH" e realizar os seguintes comandos:

    pwd --> Para analisar se estamos realmente no diretório que iniciamos nosso repositório 

    [Para lembrarmos como iniciamos o repositório - Clique AQUI](/docs/inicializandoRepositorio.md)

    Resultado esperado:
    aleite@LAPTOP-34SN20J5 MINGW64 ~/git-basico (master)

2. Analisando o status inicial do GIT - Estrutura inicial:

    Comando:
    git status

    Resultado esperado:

    On branch master  --> Significa que estamos no branch "Master".

    No commits yet    --> Não realizei nenhum commit.

    nothing to commit (create/copy files and use "git add" to track) --> Não possuo nenhum arquivo para realizar o "Commit".


3. Analisando status do git após criação de um novo arquivo - STATUS: Untacked:

    Criar um novo arquivo:   
    Comando: 
    echo TESTE > novoArquivoGit.md

    Analisar o status do git:
    
    Comando: git status

    Resultado esperado:
    On branch master

    No commits yet

    Untracked files:
    (use "git add <file>..." to include in what will be committed)
    novoArquivoGit.md   --> Podemos ver que o arquivo acabou de ser criado mas o git ainda não o reconhece.

    nothing added to commit but untracked files present (use "git add" to track)

4. Analisando status do git após adição do novo arquivo - STATUS: Unmodified e Staged :

    Comando: 
    git add novoArquivoGit.md
    
    git status
    
    Resultado esperado:
    On branch master

    No commits yet

    Changes to be committed:
    (use "git rm --cached <file>..." to unstage)

    new file:   novoArquivoGit.md   
    
    --> Como adicionamos um novo arquivo, o git entendeu e passou para um novo status "Unmodified" e Stage ou seja (pronto para realizar o "commit".

5. Analisando status do git após a realização de uma alteração do arquivo criado - STATUS: Modified:

    Alterar o conteúdo do arquivo criado (na ferramenta que desejastes).
    Validar novo status do git:

    Comando:
    git status

    Resultado esperado:
    
    On branch master

    No commits yet

    Changes to be committed:

    (use "git rm --cached <file>..." to unstage)

    new file:   novoArquivoGit.md

    Changes not staged for commit:

    (use "git add <file>..." to update what will be committed)

    (use "git checkout -- <file>..." to discard changes in working directory)

    modified:   novoArquivoGit.md   --> Conforme o esperado, tivemos uma alteração no arquivo, logo o git o passou para o status: Modified.

6. Analisando status do git após a realização de um commit:    

    Primeiramente vamos adicionar essa alteração que realizamos no nosso arquivo:
    
    git add novoArquivoGit.md

    Logo depois vamos realizar o "commit" que é momento que iremos pegar todos os arquivos do repositório e criaremos uma "imagem - uma nova versão"

    Comando:
    git commit -m "Adicionar novo arquivo de exemplo" --> -m significa que iremos adicionar um comentário.

    Resultado esperado:
    [master (root-commit) 9991ff4] Incluindo um novo arquivo de exemplo
    1 file changed, 2 insertions(+)
    create mode 100644 novoArquivoGit.md  --> Arquivo versionado com sucesso e o endereço da imagem está representado pelo identificador: 100644.

    Agora vamos analisar qual o status atual do git:
    
    Comando:
    git status:
    
    On branch master

    nothing to commit, working tree clean

* Ou seja não existe mais nada para ser feito, pois já realizamos o versionamento do nosso arquivo.


![Para um melhor entendimento seguem os Status de forma gráfica](/Imagens/git_status.jpg)