# Versionando os commits criados
## Podemos realizar o versionamento de um conjunto de funcionalidades criadas e para isso, podemos criar "tags"

Para isso, devemos executar o comando:

git tag -a 1.0.0 -m "Versão final do git-básico"    >> onde -a (iremos adicionar alguma anotação sobre qual é a versão) -m (iremos adicionar um comentário para essa versão).

git push origin master --tags    >> Tag gerada e disponibilizada.

O bacana de gerarmos tags, é que conseguimos controlar melhor o que está sendo feito. Além disso a disponibilização desse código será controlado por essa versão e irá conter apenas o que fizemos até aquele momento e quem foi o responsável pelo versionamento. Fazendo com que tenhamos um controle muito melhor de tudo que foi feito.

### Para visualizarmos quais são as tags existentes, devemos executar o comando:

git tag




