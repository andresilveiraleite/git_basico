# Visualizando Logs

## Após realizarmos o commit, podemos ter a visão do que e por quem foi feito todas as criações e alterações

Para isso, podemos utilizar o comando chamado: git log.

Resultado esperado:
commit 9991ff40d85a07d06a0481e7ddc3c80058bb00c3 (HEAD -> master) --> Identificação do Commit

Author: andresilveiraleite <teste@hotmail.com> --> Quem foi o responsável pelo Commit.

Date:   Fri Aug 18 16:50:26 2017 -0300         --> Data que o Commit foi realizado.

Incluindo um novo arquivo de exemplo           --> Mensagem que foi registrada no Commit.

Alguma

### Alguns recursos que podemos utilizar para melhorar a visualização dos logs

git log --decorate >> Exibe se as alterações foram de uma branch para a outra. Se foram geradas novas tags e quais foram essas tags, etc.

git log --author="andresilveiraleite" >> Exibe as alterações feitas apenas pelo author mencionado.

git log --shortlog  >> Exibe em ordem alfabética, quais foram os autores, quantos commits fizeram e quais foram.

git log --shortlog -sn  >> Exibe a quantidade commit e o author.

git log --graph >> Exibe de forma gráfica os branchs e as versões.

Podemos visualizar todas as informações sobre uma versão específica, utilizando a identifação que sempre é criada quando o git versiona um documento.

Para isso utilizaremos o comando: git show [ID] 






