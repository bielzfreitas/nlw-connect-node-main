# NLW Connect - Node.js

Sistema de Indicações - Referral System
- Javascript ao lado do back-end
- Quando uma pessoa se cadastra em um evento, pode fazer uma indicação para outra pessoa
- Quanto mais indicações, mais a pessoa soma pontos para o ranking
- Utilizado 2 bancos de dados diferentes

Instalar o Node.js
- baixar pelo site próprio deles (versão 18 pra cima)
- quem quiser, instala pelo package manager ou version manager
- EU utilizei o Vs Code, porém, usem qual quiser (Cursor está interessante por ter IA integrada) =)
- caso já tenha instalado, no terminal, digitar: node -v

Instalar o Docker
- um pouco (ou muito) chato de instalar, recomendo ver algum tutorial de como instalar
- caso já tenha instalado, verificar a versão pelo terminal: docker -v
- docker hub (github de docker) vários containers prontos para uso

Como identificar se o docker está funcionando
- usando o docker hub, "clonar" o hello-world
- usar este comando no temrinal: docker pull hello-world
- ele vai baixar a imagem de dentro do docker hub
- utilizar o comando: docker images
- ele lista TODAS as imagens instaladas, procure se a "hello-world" foi instalada
- para executar: docker run hello-world
- se retornar a seguinte mensagem, o docker vai estar funcionando:

---------------------------------------------------------------------------------------------

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/

---------------------------------------------------------------------------------------------

Alguns comandos do Docker
- docker ps (imagens que estão em execução)
- docker run hello-world (executa a imagem)
- docker run -d hello-world (executa em background / sem precisar ficar parando a execução toda hora)
- ele retorna a ID da imagem
- para parar a imagem: docker stop (+ ID da imagem)
- docker ps -a (mostra todas as imagens que em algum momento já foi executada, mas estão paradas no momento)
- para rodar a imagem de novo: docker start (+ ID da imagem)
