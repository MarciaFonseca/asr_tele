Responda as seguintes questões:


1. O que é um Dockerfile?

   > O Dockerfile é um arquivo de configuração utilizado para definir as instruções necessárias para criar uma imagem Docker. Ele contém uma série de comandos que são executados sequencialmente para configurar o ambiente e criar a imagem que será usada para instanciar contêineres.

2. Qual comando é usado para iniciar um Dockerfile?

   > No começo do Dockerfile usa-se o comando `FROM`. Para criar uma imagem a partir de um Dockerfile usa-se o comando `docker build -t nomedaimagem:tag`.

3. Qual comando é usado para definir a imagem base no Dockerfile?

   > `FROM`.

4. Como você adiciona arquivos locais ao sistema de arquivos do contêiner no Dockerfile?

   > `COPY`.

5. Como você especifica o diretório de trabalho no Dockerfile?

   > `WORKDIR`.

6. Qual comando é usado para executar comandos durante a criação da imagem Docker no Dockerfile?

   > `RUN`.

7. Como você expõe portas no Dockerfile?

   > `EXPOSE`.

8. Qual comando é usado para definir variáveis de ambiente no Dockerfile?

   > `ENV`.

9. Como você comenta linhas no Dockerfile?

   > `Basta comentar com #`.

10. Qual comando é usado para executar a aplicação principal quando um contêiner é iniciado no Dockerfile? start/stop.

    > `CMD`.

11. Responda: O Docker usa uma interface CLI para gerenciar os seus vários objetos através de comandos. O que faz os comandos abaixo:  
    1. `docker run`:

       > é usado para executar um container Docker.

    2. `docker build`:

       > é usado para construir uma imagem.

    3. `docker pull`:

       > é usado para baixar uma imagem Docker de um repositório remoto, como o Docker Hub.

    4. `docker push`:

       > enviar imagens de contêiner para um repositório.

    5. `docker ps`:

       > é usado para listar todos os containers Docker em execução no *host*.

    6. `docker images`:

       > é usado para listar todas as imagens que estão armazenadas no host Docker local.

    7. `docker stop`:

       > é usado para parar a execução de um container Docker em execução.

    8. `docker start`:

       > é usado para iniciar a execução de um container Docker que foi previamente criado.

    9. `docker rm`:

       > é usado para remover um container Docker.

    10. `docker rmi`:

        > é usado para remover uma imagem Docker do *host* local.

    11. `docker exec`:

        > é usado para executar um comando dentro de um container que já está em execução.

    12. `docker logs`:

        > é usado para exibir os *logs* de um container que já está em execução.

    13. `docker network`:

        > é usado para gerenciar redes. 

    14. `docker volume`:
   
        > é usado para gerenciar volumes.


Registre as respostas a esse questionário do seu GitHub e poste o *link* da atividade no Classroom.
