# git revert
## Podemos utilizar esse comando quando queremos reverter para o código anterior, mas não gostaríamos de "remover" o que foi feito


1. Alterar um arquivo
2. Realizar o commit dessa alteração
3. Executar o comando "git log" para resgatar o identificar do commit que realizamos acima 
4. Realizar o comando: 

    git revert [identificador do commit - pego no passo 3]


    Pronto, conseguimos voltar para a versão estável e podemos retomar a versão que estava ocasionando erro num momento oportuno.