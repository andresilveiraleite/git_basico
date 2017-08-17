# Inicializando um novo Repositório
## Para inicializar um novo repositório, é necessários seguir alguns passos:

1. Criar Pasta para o novo projeto:

   Executar o comando:
    mkdir git-basico

2. Acessar pasta criada:

   Executar o comando: 
    cd git-basico

3. Inicializar um repositório:
   
   Executar o comando:
    git init   
    --> Esse comando, será responsável por inicializar o repositório e fica monitorando todas as mudanças que estiverem dentro desse projeto.

    A mensagem exibida após esse comando é algo parecido com:
    
    Initialized empty Git repository in C:/Users/aleite/git-basico/.git/

4. Validando se o repositório realmente foi inicializado:
    
    Execute o comando:
    ls -la
    
    A mensagem exibida após esse comando é algo parecido com:
    
    drwxr-xr-x 1 aleite 197121 0 ago 17 17:34 ./

    drwxr-xr-x 1 aleite 197121 0 ago 17 17:30 ../

    drwxr-xr-x 1 aleite 197121 0 ago 17 17:34 .git/

5. Entendendo a Estrutura criada pelo GIT:
    
    Percebemos na etapa anterior que existe uma pasta com o nome .git, vamos acessá-la:

    Execute os comandos abaixo:

    cd .git

    ls -l

    Deve ser exibido a estrutura do git (exemplificado logo abaixo):

    -rw-r--r-- 1 aleite 197121 130 ago 17 17:34 config

    -rw-r--r-- 1 aleite 197121  73 ago 17 17:34 description

    -rw-r--r-- 1 aleite 197121  23 ago 17 17:34 HEAD

    drwxr-xr-x 1 aleite 197121   0 ago 17 17:34 hooks/

    drwxr-xr-x 1 aleite 197121   0 ago 17 17:34 info/

    drwxr-xr-x 1 aleite 197121   0 ago 17 17:34 objects/

    drwxr-xr-x 1 aleite 197121   0 ago 17 17:34 refs/

    Essas pastas são responsáveis por guardar a configuração do repositório, qual é o branch padrão, quais os branchs existentes no meu projeto + Descrições, hooks (Gatilhos para executar algumas ações) e outras referências.





