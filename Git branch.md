
O comando git branch e utilizado para criar partições no projeto, sendo assim, temos a parte principal que é o master, sendo possivel criar uma partição a parte

Sendo assim, ao criar uma branch é possivel saber o que cada um realizou

comando

git branch <nome da branch>

para verificar se funcionou digite:
git branch

Para entrar na branch:

git branch checkout <nome da branch>

Se uma outra pessoa que for colaboradora, criar uma branch e realizar uma alteração, essa alteração somente será visualizada no computador dela, assim como a branch que criou, ao  realizar um push, um  solicitação será enviada para o repositorio remoto, para que o  master, o dono do repositorio autorize, caso o aprove, basta clicar 

Para exemplificar, criei um branch chamada teste:

PS C:\Users\PauloFialho\Downloads\appdequiz> git branch teste2
PS C:\Users\PauloFialho\Downloads\appdequiz> 

Para que as alterações sejam enviadas para a branch, assim que os commits será nescessario entrar nesse branch

PS C:\Users\PauloFialho\Downloads\appdequiz> git checkout teste2
Switched to branch 'teste2'

Para saber se está na branch correta utilize o comando git branch, a branch que estiver destacada em verde ou como asterisco do lado será a branch onde está

PS C:\Users\PauloFialho\Downloads\appdequiz> git branch
  checkout
  master
  novorecurso
  teste
* teste2

Para fins de exemplificação, realizei uma alteração ao acaso no projeto, mudei a cor do background para preto,  logo em seguida uso o git add .  e logo em seguida faça um commit, depois realize um push

PS C:\Users\PauloFialho\Downloads\appdequiz> git add .
PS C:\Users\PauloFialho\Downloads\appdequiz>  git commit -m "mudando a cor"
[teste2 69f86ac] mudando a cor
 1 file changed, 1 insertion(+), 1 deletion(-)


git push origin master

fatal: The current branch teste2 has no upstream branch.      
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin teste2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

O erro acontece devido que não estamos mais na branch master, mas na branch que criamos a teste2, sendo assim o push é conforme a orientação dada:

 git push --set-upstream origin teste2

Após executar o comando, será enviada para o repositorio remoto

No repositorio remoto, no repositorio do seu projeto, terá uma informação que algume realizou uma banch no projeto, para que alterações sejam anexadas ao projeto principalm o master, ou seja, o dono do repositorio ou lider, deverpa analisar a alteração e aceita-la ou rejeita-la.

No github aparecerá de duas maneiras, na tela principal como um aviso na parte superiror, ou clicando em branches


conforme a imagem, clique nela
![[Pasted image 20231106124655.png]]

Clique no icone das branches, e na branches clique em pull requests

adicione um titulo
escreva um comentario e clique em create pull requests

Role e busque por merge pull requests, esse comando vai fazer com a alteração da branch principal seja enviada para o branch, confime e se aparece o icone da branch em roxo, significa que alteração foi realizada


