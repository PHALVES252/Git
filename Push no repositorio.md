
Push é o mesmo que enviar um projeto para oi repositorio

Vamos fazer isso via linha de comando

primeiro crie um projeto na ide que desejar, utilizando o comando cd, siga até a pasta do projeto que criou

Abra o cmd e digite  git  init  para iniciar o repositorio, ao clicar em enter irá aparecer uma mensagem que o repositorio foi iniciado, esse comando irá criar uma pasta chamada git no projeto que criou

Digite git add *,  irá passar pela tela varias linhas de codigos, porem isso não é regra

Para realizar o primeiro commit digite git commit -m "commit inicial"
Para saber se foi realizado o comit digite git log
Importante, esse comando só irá funcionar apenas uma vez

IPORTANTE: O GIT COMMIT SÓ IRÁ FUNCIONAR SE ANTES HOUVE O GIT ADD *

Agora finalmente para enviar seu projeto para o o github, primeiro crie um repositorio, no github, logado na conta, no canto esquerdo da tela clique em "NEW"

Em repository name, crie um nome, caso deseje em description escreva um descrição sobre o repositorio

Marque a opção se o repositorio irá estar publico ou privado

Clique em create repository, irá criar um repositório vazio, porem assim que criar, haverá varias informações sobre como gerenciar o repositório.

Nesse mesma pagina haverá um codigo já pronto de como informar qual repositorio o github fará conexão

git remote add origin https://github.com/PHALVES252/aulaGit.git

Não irá surgir nenhuma informação, mas o comando remoto será iniciado

Para mandar, ou fazer um push do projeto que realizou basta digitar 
*git push origin master*

origin pé o repositorio remoto, ou seja seu computador onde os codigos do projeto se encontrm
Master é o repositorio no github