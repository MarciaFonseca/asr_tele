O Dockerfile é um arquivo de configuração utilizado para definir as instruções necessárias para criar uma imagem Docker. Ele contém uma série de comandos que são executados sequencialmente para configurar o ambiente e criar a imagem que será usada para instanciar contêineres. Responda as seguintes questões:


1. O que é um Dockerfile?

   > O Dockerfile é um arquivo de configuração utilizado para definir as instruções necessárias para criar uma imagem Docker. Ele contém uma série de comandos que são executados sequencialmente para configurar o ambiente e criar a imagem que será usada para instanciar contêineres.

2. Qual comando é usado para iniciar um Dockerfile? docker build -t

3. Qual comando é usado para definir a imagem base no Dockerfile? FROM

4. Como você adiciona arquivos locais ao sistema de arquivos do contêiner no Dockerfile? COPY

5. Como você especifica o diretório de trabalho no Dockerfile? WORKDIR 

6. Qual comando é usado para executar comandos durante a criação da imagem Docker no Dockerfile? docker build -t <imagem>

7. Como você expõe portas no Dockerfile? EXPOSE

8. Qual comando é usado para definir variáveis de ambiente no Dockerfile? Docker run

9. Como você comenta linhas no Dockerfile? basta comentar com # 

10. Qual comando é usado para executar a aplicação principal quando um contêiner é iniciado no Dockerfile? start/stop.

11. Responda: O Docker usa uma interface CLI para gerenciar os seus vários objetos através de comandos. O que faz os comandos abaixo:  
    1. `docker run`:
        é usado para executar um container Docker.
    2. `docker build`:
        Antes de mais nada, para usarmos este comando, é necessário a criação de um Dockerfile. Para exemplo, criaremos um simples que instala o servidor web Nginx e copia um arquivo HTML para o diretório padrão do servidor web: e então ele constrói uma imagem a partir de um Dockerfile e de um contexto
    3. `docker pull`:
        é usado para baixar uma imagem Docker de um repositório remoto, como o Docker Hub.
    4. `docker push`:
        enviar imagens de contêiner para um repositório
    5. `docker ps`:
        é usado para listar todos os containers Docker em execução no host
    6. `docker images`:
        é usado para listar todas as imagens que estão armazenadas no host Docker local
    7. `docker stop`:
        é usado para parar a execução de um container Docker em execução
    8. `docker start`:
         é usado para iniciar a execução de um container Docker que foi previamente criado e parado
    9. `docker rm`:
        é usado para remover um container Docker que não está mais em execução.
    10. `docker rmi`:
         é usado para remover uma imagem Docker do host local.
    11. `ndocker exec`:
         é usado para executar um comando dentro de um container que já está em execução
    12. `docker logs`:
          é usado para exibir os logs de um container que já está em execução.
    13. `docker network`:

    14. `docker volume`:

Registre as respostas a esse questionário do seu GitHub e post o Link da atividade no Classroom.
