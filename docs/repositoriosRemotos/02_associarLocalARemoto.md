# Associar repositório Local ao Github
## Após a criação de um repositório remoto, precisamos associar o mesmo ao nosso local


* Primeiramente, devemos salientar que para executar os passos abaixo, devemos estar num prompt de comando no diretório aonde nosso projeto local encontra-se.


    Para isso, podemos utilizar o próprio comando que o git recomenda:

    git remote add origin git@github.com:[nomeDoUsuarioDoGit]/github-course.git

    Para confirmar que foi associado iremos realizar o seguinte comando:

    git remote >> Exibirá que já existe o repositório "origin"

    git remote -v >> Exibirá o endereço do repositório remoto.

    Logo depois iremos executar o último comando - git push -u origin master. 

    Ele enviará todos os arquivos que possuímos, todas as modificações, logs, etc para o repositório que estamos determinando. 

    É importante citar que o "-u origin master" será utilizado apenas na 1 x, pois nele confirmamos pra onde vai e de onde vem, logo, vem do branch master (branch padrão - quando iniciamos no githu) e vai para o origin.



* Após a realização dos procedimentos acima, ao acessarmos novamente o github (darmos um refresh na página), passaremos a enxergar o nosso projeto local, de forma remota.


