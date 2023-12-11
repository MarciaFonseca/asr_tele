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

   > <a name="fig-01"></a>![01](img/01.png)
     ***Figura 1**. Criação dos diretórios e do arquivo `mosquitto.conf`.*

   > ---

   > <a name="fig-02"></a>![02](img/02.png)
     ***Figura 2**. Conteúdo do `compose.yml`.*

   > ---

   > <a name="fig-03"></a>![03](img/03.png)
     ***Figura 3**. Conteúdo do `compose.yml` (continuação).*

   > ---

   > <a name="fig-04"></a>![04](img/04.png)
     ***Figura 4**. Execução do `docker compose up --detach`.*

   > ---

   > <a name="fig-05"></a>![05](img/05.png)
     ***Figura 5**. Execução do `docker compose up --detach` (continuação).*

   > ---

   > <a name="fig-06"></a>![06](img/06.png)
     ***Figura 6**. Inserção do caminho para o arquivo `passwd` contendo a senha.*

   > ---

   > <a name="fig-07"></a>![07](img/07.png)
     ***Figura 7**. Portas 1883, 8123 e 9001 abertas no Play with Docker.*

   > ---

   > <a name="fig-08"></a>![08](img/08.png)
     ***Figura 8**. Página de boas-vindas do Home Assistant.*

   > ---

   > <a name="fig-09"></a>![09](img/09.png)
     ***Figura 9**. Criação do usuário `gabriel-marcia-pablo`.*

   > ---

   > <a name="fig-10"></a>![10](img/10.png)
     ***Figura 10**. Inserção da localização no Home Assistant.*

   > ---

   > <a name="fig-11"></a>![11](img/11.png)
     ***Figura 11**. Pedido de permissões do Home Assistant.*

   > ---

   > <a name="fig-12"></a>![12](img/12.png)
     ***Figura 12**. Identificação de dispositivos no Home Assistant.*

   > ---

   > <a name="fig-13"></a>![13](img/13.png)
     ***Figura 13**. Página inicial do Home Assistant.*

   > ---

   > <a name="fig-14"></a>![14](img/14.png)
     ***Figura 14**. Lista de compras no Home Assistant, inicialmente vazia, que será usada para testar o envio de mensagens pelo MQTT.*

   > ---

   > <a name="fig-15"></a>![15](img/15.png)
     ***Figura 15**. Edição da lista de compras.*

   > ---

   > <a name="fig-16"></a>![16](img/16.png)
     ***Figura 16**. Edição da lista de compras (continuação).*

   > ---

   > <a name="fig-17"></a>![17](img/17.png)
     ***Figura 17**. Lista de compras renomeada para "A fazer".*

   > ---

   > <a name="fig-18"></a>![18](img/18.png)
     ***Figura 18**. Menu de configurações do Home Assistant. Neste menu, foi selecionado o item "Automações & Cenas".*

   > ---

   > <a name="fig-19"></a>![19](img/19.png)
     ***Figura 19**. Página de configuração de automações. Foi selecionado  "+ Criar automação" no canto inferior direito.*

   > ---

   > <a name="fig-20"></a>![20](img/20.png)
     ***Figura 20**. Opções para a criação de automação. Selecionada a primeira opção: "Criar nova automação".*

   > ---

   > <a name="fig-21"></a>![21](img/21.png)
     ***Figura 21**. Configuração de automação para acrescentar 3 itens à lista "A fazer" ao receber, por MQTT, a mensagem "atribuir" vinculada ao tópico "asr/nota".*

   > ---

   > <a name="fig-22"></a>![22](img/22.png)
     ***Figura 22**. Continuação da configuração de automação. Detalhes do primeiro item aa ser acrescentado à lista.*

   > ---

   > <a name="fig-23"></a>![23](img/23.png)
     ***Figura 23**. Continuação da configuração de automação. Detalhes do segundo item aa ser acrescentado à lista.*

   > ---

   > <a name="fig-24"></a>![24](img/24.png)
     ***Figura 24**. Continuação da configuração de automação. Detalhes do terceiro item aa ser acrescentado à lista.*

   > ---

   > <a name="fig-25"></a>![25](img/25.png)
     ***Figura 25**. Automação salva com o nome "atribuir-nota".*

   > ---

   > <a name="fig-26"></a>![26](img/26.png)
     ***Figura 26**. Resumo da automação "atribuir-nota".*

   > ---

   > <a name="fig-27"></a>![27](img/27.png)
     ***Figura 27**. Integração com MQTT.*

   > ---

   > <a name="fig-28"></a>![28](img/28.png)
     ***Figura 28**. Configuração do MQTT. O "Endereço do Broker" corresponde ao endereço IP disponibilizado pelo Play with Docker. Foi usada a porta 1883, porta padrão do MQTT, vide [Figura 7](#fig-07). Os campos usuário e senha foram preenchidos conforme a configuração feita no contêiner do eclipse-mosquitto (MQTT), vide [Figura 6](#fig-06).*

   > ---

   > <a name="fig-29"></a>![29](img/29.png)
     ***Figura 29**. Integração com MQTT configurada com sucesso.*

   > ---

   > <a name="fig-30"></a>![30](img/30.png)
     ***Figura 30**. Página de integração do Home Assistant com o MQTT. Selecionado o item "Configurar", à direita.*

   > ---

   > <a name="fig-31"></a>![31](img/31.png)
     ***Figura 31**. Publicação e escuta de um pacote para o tópico `asr/nota` com a mensagem `atribuir` (também chamada de valor ou payload, 'carga útil' em inglês). Evidencia-se o funcionamento do MQTT pelo processo de publicação e assinatura (publish/subscribe, PUB/SUB).*

   > ---

   > <a name="fig-32"></a>![32](img/32.png)
     ***Figura 32**. O envio do pacote por MQTT para o tópico `asr/nota` com a mensagem `atribuir` (vide [Figura 31](#fig-31)) ativou o gatilho da automação `atribuir-nota` anteriormente configurada (vide [Figuras 21](#fig-21), [22](#fig-22), [23](#fig-23), [24](#fig-24), [25](#fig-25) e [26](#fig-26)), acrescentando 3 itens à lista "A fazer".*

   > A execução desta atividade avaliativa pode ser assistida no vídeo "Automação com Docker Compose, MQTT e Home Assistant" elaborado pela equipe e disponível em: https://youtu.be/mGhKJEOL_Pg<br>
   > [![Automação com Docker Compose, MQTT e Home Assistant](https://markdown-videos-api.jorgenkh.no/url?url=https%3A%2F%2Fyoutu.be%2FmGhKJEOL_Pg)](https://youtu.be/mGhKJEOL_Pg).
