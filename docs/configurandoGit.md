# Configurando o GIT
## Definição do usuário/e-mail e editor de código

O git armazena as informações em 3 lugares:

1. Git config do sistema
2. git config do usuário 
3. git config do projeto (específico daquele repositório)

### Configuração do Usuário:

Definindo Usuário:
git config --global user.name "André Leite"

Definindo E-mail:
git config --global user.email "asmla@hotmail.com"

Definindo o Editor de preferência do usuário:
git config --global core.editor visual studio --> Ou sub (sublime) ou vim.
Obs.: Se não for definido o editor de sua preferência, o git por padrão utilizará o "VIM".


#### Para sabermos quais foram os parâmetros que foram definidos, temos duas maneiras:
 
* Resgatar a informação de maneira específica:

git config user.name    --> Exibirá o nome que foi definido.

git config user.email   --> Exibirá o e-mail que foi definido.

* Resgatar todas as informações que foram definidas:

git config --list       --> Listará todos os parâmetros que foram definidos no git.
