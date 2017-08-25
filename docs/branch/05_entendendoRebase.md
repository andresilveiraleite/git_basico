# Entendendo Rebase
## Além do merge, podemos utilizar para união dos commits, uma funcionalidade muito bacana, o "Rebase".

Vamos levar em consideração o seguinte cenário: 
2 branchs (master e testes) e 3 commits(C0, C1 e C2).

![Cenário de teste - Rebase](/Imagens/rebase.jpg)


Além disso cada branch citado acima possui um commit independente
(A partir do C2> C3 --> testes e A partir do c2> C4--> Master)

* Levem em consideração que gostaríamos de unir os commits dos branchs testes (C3) e master (C4):

A grande diferença do merge para o rebase está exatamente na maneira que ele une os commits. No merge teríamos a criação de um novo branch para unir o commit 3 e o 4, no rebase teremos a movimentação do commit 3 para frente do commit 4, logo teremos algo mais linear e sem a permanência de um commit desnecessário.


![Ex. Rebase sendo executado:](/Imagens/rebaseAcionado.jpg) 


### Prós:
Evita criação de commit desnecessário.

Histórico Linear > Semmpre teremos a movimentação de um commit para frente do processo e evitaremos a confusão que é gerada pelo método "merge".

#### Contras:
Perdemos a ordem cronológica, pois nosso commit sempre se movimenta para frente do processo e com isso mudamos o histórico, logo se alguma pessoa estiver num mesmo branch. 

sempre que for dar pull das modificações, é indicado o rebase e para isso, podemos executar o seguinte comando:

git pull --rebase (assim não corremos risco de realizar mudanças de histórico em que outras pessoas estejam manipulando).

