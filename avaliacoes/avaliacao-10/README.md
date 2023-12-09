<p align="center">
    <picture>
        <source media="(prefers-color-scheme: dark)" srcset="/img/ifce/logo-vertical-branca_media.png">
        <source media="(prefers-color-scheme: light)" srcset="/img/ifce/logo-vertical-colorida_media.png">
        <img alt="IFCE" width="100" src="/img/ifce/logo-vertical-colorida_media.png">
    </picture>
</p>

<p align="center"><b>INSTITUTO FEDERAL DE EDUCAÇÃO, CIÊNCIA E TECNOLOGIA DO CEARÁ</b><br>
<b><i>CAMPUS</i> FORTALEZA</b><br>
<b>TECNOLOGIA EM TELEMÁTICA</b></p>

<p align="center">
CARLOS GABRIEL SACRAMENTO<br>
CÍCERA MÁRCIA DA FONSECA SILVA<br>
PABLO BUSATTO</p>

<p align="center">2 de dezembro de 2023</p>

# Avaliação 10 – MQTT

1. O MQTT (*Message Queuing Telemetry Trasport*) é um protocolo leve que implementa o modelo de transporte PUB/SUB (*publish*/*subscribe*). Esse modelo é usado em aplicações de mensageria. O MQTT é principalmente usando em aplicações IoT (internet das coisas). Essa atividade tem como objetivo implementar uma aplicação MQTT usando o `docker-compose`.
Evidenciar o funcionamento da aplicação usando *prints*. Sugerimos usar o [Play with Docker](https://labs.play-with-docker.com) com o `docker-compose`. Observar os *links* de artigos apresentando esse tema, anexos abaixo. Trabalho com equipes de no máximo três alunos.

   > ![1](https://github.com/PabloBF/asr_tele/assets/55034604/411f9493-7b17-484d-88cb-3d95d51b1c5f)
     ***Figura 1**. Instalação do Mosquitto pelo `docker-compose`.*

   > ---

   > ![2](https://github.com/PabloBF/asr_tele/assets/55034604/53ebc0b0-280b-45b1-a391-dcfa8bd58827)
     ***Figura 2**. Conteúdo do `docker-compose.yaml`.*

   > ---

   > ![3](https://github.com/PabloBF/asr_tele/assets/55034604/458787c0-0895-4d48-b6e3-610373b15330)
     ***Figura 3**. Página do Portainer.*

   > ---

   > ![4](https://github.com/PabloBF/asr_tele/assets/55034604/99e67158-0dcf-401c-813b-d16c78ca05ec)
     ***Figura 4**. Ambientes no Portainer.*

   > ---

   > ![5](https://github.com/PabloBF/asr_tele/assets/55034604/d7fd69a9-2159-4c5f-bf90-73ee6e722972)
     ***Figura 5**. Lista de contêiners, com `homeassistant`, `mosquitto` e `portainer` em execução.*
   
   > ---
   
   > ![6](https://github.com/PabloBF/asr_tele/assets/55034604/5b20ad71-8f13-4d2e-bd02-c89035e49365)
     ***Figura 6**. Detalhes da configuração do contêiner `homeassistant`.*

   > ---

   > ![7](https://github.com/PabloBF/asr_tele/assets/55034604/acc969df-9c6a-4514-b978-4a8c9f6a70a4)
     ***Figura 7**. Configuração da porta no `homeassistant`.*

   > ---

   > ![8](https://github.com/PabloBF/asr_tele/assets/55034604/f8adfef5-31c7-4f65-87e7-e87add601be4)
     ***Figura 8**. Portas acessíveis pelo Play with Docker.*

   > ---

   > ![9](https://github.com/PabloBF/asr_tele/assets/55034604/5aefbcb4-f6b5-4673-bd88-b263e6141662)
     ***Figura 9**. Home Assistant configurado e exibindo a localização do IFCE e os integrantes da equipe.*
