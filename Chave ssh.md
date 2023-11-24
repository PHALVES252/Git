Primeiramente será nescessario que crie um conta no git hub, logo em seguida, para que os projetos que forem criados seja protegidos crie uma chave SSH no github

A chave ssh identifica seu computador que realizar os commites(comentarios), basicamente para que se autenticar( dizer que é voce  mesmo)

Para cria-la, há um texto no github ensinando como faz , basta clicar na foto do seu perfil, descer até gitbub docs, logo em seguida pesquise por SSH

1. Abra Git Bash. (Pode ser pelo terminal do windows)
    
2. Cole o texto abaixo, substituindo o email usado no exemplo pelo seu endereço de email GitHub.
    
    ```shell
    ssh-keygen -t ed25519 -C "your_email@example.com"
    ```

o resultado no meu caso com "oclubedosdez@gmail.com" é

![[Pasted image 20231028104353.png]]

clique duas vezes e coloque um senha caso deseje, o resultado será um serie de carcteres com numero da chave

Serão criadas duas chaves, uma publica e outra privadas, ela estaram no caminho indicado no print acima

para gerar um chave publica, para que o github saiba que sou eu que está fazendo os comits, no caminho indicado para a pasta ssh, clique na chave publica, copie o codigo

Volte no github clique na foto de perfil e clique em setings, no canto esquerdo da tela clique em " SSH AND GPG KEYS"

Em SSH kEYS  clique no botão verde "New SSH kEYS"

Escolha um titulo que desejar, em key, cole o codigo que copiou da chave publicar e confirme

chave criada

