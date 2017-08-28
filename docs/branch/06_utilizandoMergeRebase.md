# Utilizando o Merge e Rebase
## Agora vamos colocar em prática os conceitos de Merge e Rebase.
### Levaremos em consideração que esse repositório local encontra-se associado ao remoto


#### Exemplificando o MERGE:




1. Criar Nova Pasta e Inicializar repositório:

    mkdir rebase-merge-pratica  >> Cria uma nova pasta

    Acessar pasta criada:

    cd rebase-merge-pratica

    Inicializar o repositório:

    git init

2. Criar arquivo no branch "padrão - Master", adicionar e commitar:

    echo MasterArq1 > arqTestes1.md     >> Criando arquivo 1

    git add *   >> Adicionando os novos arquivos

    git commit -m "novo arquivo 'arqTestes1.md' para o master"  


3. Criar um novo branch "merge_branch" e adicionar um novo arquivo para o mesmo:

    git checkout -b merge_branch

    echo TestesArq2 > arqTestes2.md     >> Criando arquivo 2
    
    git add *   >> Adicionando o novo arquivo

    git commit -m "novo arquivo 'arqTestes2.md' para o merge_branch" 


4. Criar arquivo no branch "padrão - Master", adicionar e commitar:

    echo MasterArq3 > arqTestes3.md     >> Criando arquivo 3

    git add *    >> Adicionando o novo arquivo

    git commit -m "novo arquivo 'arqTestes3.md' para o branch master"  


5. Executando o merge no commit contendo o arquivo "arqTestes2.md" (branch merge_branch) para o branch "master"

    git checkout master  >> Mudar para o brach "master"

    git merge merge_branch    >> O arquivo "arqTestes2.md" (branch: merge_branch) será incluído no branch master e o histórico será mantido de forma linear. Lembrando que teremos um novo commit só para esse junção (uma característica do "merge").



#### Exemplificando o REBASE:




1. Criar novo arquivo no branch "padrão - Master", adicionar e commitar:

    echo MasterArq4 > arqTestes4.md     >> Criando arquivo 4

    git add *    >> Adicionando o novo arquivo

    git commit -m "novo arquivo 'arqTestes4.md' para o branch master"  


2. Criar um novo branch "rebase_branch" e adicionar um novo arquivo para o mesmo:

    git checkout -b rebase_branch

    echo TestesArq5 > arqTestes5.md     >> Criando arquivo 5

    git add *    >> Adicionando o novo arquivo

    git commit -m "novo arquivo 'arqTestes5.md' para o branch rebase_branch"


3. Acessar branch "master" e adicionar um novo arquivo para o mesmo:

    git checkout master

    echo TestesArq6 > arqTestes6.md     >> Criando arquivo 6

    git add *    >> Adicionando o novo arquivo

    git commit -m "novo arquivo 'arqTestes6.md' para o branch master"
    
4. Executando o merge no commit contendo o arquivo "arqTestes5.md" (branch rebase_branch) para o branch "master"

    git checkout master  >> Mudar para o brach "master"

    git merge rebase_branch    >> O arquivo "arqTestes5.md" (branch: rebase_branch) 

Importante citar que não foi criado um novo commit, ele simplesmente moveu a alteração para o topo da lista. 
Muitos recomendam a utilização do rebase.


* Disponibilizaremos em breve a codificação desse exemplo, para ficar mais simples o entendimento. 

