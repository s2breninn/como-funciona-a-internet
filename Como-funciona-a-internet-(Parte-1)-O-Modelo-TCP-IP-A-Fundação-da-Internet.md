# Como funciona a internet (Parte 1): O Modelo TCP/IP: A Fundação da Internet

- Parte 1: O Modelo TCP/IP: A Fundação da Internet
- Parte 2: HTTP: A Linguagem da WEB
- Parte 3: Segurança na Internet: Protegendo os Dados 
- Parte 4: DNS e Roteamento: Os Nomes da Internet  
  

Para responder a pergunta "Como funciona a internet?", é importante que você saiba o que ela é.
O que chamamos de _internet_ é uma conexão entre multiplos dispositivos de comunicação, seja por cabo ou não.

Mas para que eles possam se comunicar, todos precisam "falar a mesma lingua".
Por isso, alguns __protocolos__ de comunicação foram criados como o __UDP__ e o que vamos falar hoje: O Protocolo __TCP__.

## Protocolos e Pacotes
Antes de mergulharmos no TCP, é importante entender o que são protocolos e pacotes, dois conceitos fundamentais na comunicação pela internet.

Um protocolo é em resumo, um conjunto de regras que vai definir como os dados são transmitidos e recebidos.
É tipo a gramática: ele dita formatos e estruturas de informação para que todos os envolvidos se entendam.

E quando uma mensagem vai ser enviada de um dispositivo para o outro, ela é dividida em pacotes que serão remontados quando chegarem ao destino.

Tenha isso em mente para poder entender o próximo tópico.

## O TCP
__TCP__, que significa __Transmission Control Protocol__ (Protocolo de Controle de Transmissão), é um dos principais protocolos de comunicação na Internet por sua segurança de comunicação
E isso é porque ele trabalha com garantias.

Antes de enviar qualquer informação, ele estabelece a conexão com o destino e aguarda uma resposta.
Esse passo, nós chamamos de "handshake", ou em bom português: "Aperto de mão".

TCP Hanshake

Uma vez que a conexão foi garantida, ele começa o envio dos pacotes de maneira ordenada recebendo uma confirmação para cada pacote recebido.

E o mais importante: caso o dispositivo não receba a confirmação de recebimento, ele vai reenviar aquele mesmo pacote, garantindo que todos os dados cheguem intactos e na ordem correta.

## O UDP
__UDP__, que significa __User Datagram Protocol__ (Protocolo de Datagrama do Usuário), é outro protocolo que é conhecido por sua eficiência e velocidade.

Diferente do TCP, o UDP não estabelece uma conexão antes de enviar informações.
Ele simplesmente envia os pacotes de dados sem sequer saber se vai ser recebido ou não.
Esse processo é conhecido como "fire and forget", ou "dispare e esqueça".

Meme UDP

Sem o processo de confirmações, o UDP consegue enviar pacotes de dados muito mais rapido do que o TCP.

Mas com isso, não existe nenhuma garantia de que todos os pacotes foram recebido ou mesmo que foram ordenados na sequencia correta.

Apesar disso, o UDP é ideal para situações em que a velocidade é mais importante do que a confiabilidade, como transmissões de vídeo ao vivo ou jogos online.

## Conclusão sobre TCP e a transição para HTTP
Entendendo as funções do TCP e do UDP, fica claro porque o TCP é tão importante para garantir uma comunicação segura e eficiente na internet.

Através de desse processo burocrático de "handshake" e confirmações, o TCP garante que cada pacote de informação alcance seu destino em perfeita ordem.

Mas a história não acaba aqui.

Ainda precisamos falar sobre como esses dados são apresentados e interagem em um ambiente web.
E é aí que o __HTTP__ (Hypertext Transfer Protocol) entra em cena.

Ele molda a forma como as informações são trocadas e compreendidas entre os navegadores e servidores.

 Fonte: https://racoelho.com.br/posts/como-funciona-a-internet-parte-1