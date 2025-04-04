# REVISãO PROVA - I.E.S.G.O  

## Aluno : Luan B S C
## Professor : JP Gress


```txt
* Lembrete OSI *
   * 1 ~ 7 * 

Camada Física
Camada de Enlace de Dados
Camada de Rede
Camada de Transporte
Camada de Sessão
Camada de Apresentação
Camada de Aplicação


Camada física: Define o meio físico de comunicação e as tecnologias para transmitir dados 
Camada de enlace de dados: Define a funcionalidade das camadas inferiores 
Camada de rede: Define os padrões e protocolos de roteamento 
Camada de transporte: Divide os dados em segmentos menores, garantindo que eles sejam transmitidos corretamente e reagrupados no destino 
Camada de sessão: Responsável por estabelecer, manter e encerrar sessões de comunicação 
Camada de apresentação: Faz parte do modelo OSI 
Camada de aplicação: Faz parte do modelo OSI 
```



## 1. Uma empresa de tecnologia está implementando uma nova infraestrutura de rede para melhorar a comunicação entre seus servidores. Durante o processo, um engenheiro de redes explica que a camada de enlace de dados desempenha um papel fundamental na conversão de pacotes em quadros ou células para transmissão, garantindo o endereçamento correto e a integridade dos dados. Ele menciona que alguns protocolos utilizam quadros de tamanho variável, enquanto outros utilizam células de tamanho fixo
```txt
## R : A camada de enlace realiza a conversão de pacotes em quadros, adicionando endereços de origem e destino, controle de erros e fragmentação quando necessário.

### Entendimento : camada de enlace de dados é a responsavel pelo desempenho da rede , ela converte pacotes em quadros adicione endereço controla erro e fragmenta quando precisa .
```
---------------------------------------------------------------------------------------------------------------------------

## 2. Uma equipe de administradores de rede está configurando um novo ambiente de comunicaçã para uma empresa. Durante a configuração, um dos técnicos explica que a camada de enlace dedados gerencia o meio de transmissão e controla o acesso, garantindo que os dispositivospossam enviar dados sem colisões. Além disso, ele menciona que essa camada opera sobprotocolos específicos e é controlada principalmente por hardware, enquanto as camadassuperiores dependem de software.
```txt
## R : A camada de enlace gerencia o meio de transmissão e controla o acesso, garantindo que os dispositivos só transmitam quando o meio estiver disponível.

### Entendimento : A camada de enlace gerencia os dipositivos por meio dos endereços MAC's Garantindo ordem entre transmissões.
( Ultiliza Token Ring e CSMA/CD (Ethernet) para esse controle.
Garante a entrega livre de erros entre dois nós ) 
ATUAL NO HARDWRE DAS PLACAS DE REDES.
```
---------------------------------------------------------------------------------------------------------------------------
## 3. Uma empresa está implementando uma rede sem fio para conectar seus dispositivos móveis e garantir uma comunicação eficiente. Durante a configuração, um engenheiro de redes explica que, ao contrário da maioria das redes cabeadas, o Wi-Fi utiliza um mecanismo de confirmação para garantir a entrega correta dos quadros. Esse mecanismo envolve o envio de uma mensagem de reconhecimento (ACK) para confirmar a recepção bem-sucedida dos dados.

```txt
## R : A confiabilidade na transmissão pode ser implementada na camada de enlace, mas geralmente é delegada à camada de transporte.

### Entendimento : O ACK é um protocolo que atual em rede WI-FI e ele garante a entrega tem tratamento de erros e transmissao garantida EX: TPC 

```
---------------------------------------------------------------------------------------------------------------------------
## 4. Uma empresa está expandindo sua infraestrutura de rede e precisa decidir sobre a melhor abordagem para conectar seus dispositivos. O administrador de redes explica que switches desempenham um papel fundamental na comunicação em redes cabeadas, operando na camada 2 e utilizando endereços MAC para gerenciar o tráfego de dados. Ele também menciona que tanto redes cabeadas quanto sem fio utilizam o protocolo LLC (IEEE 802.2), mas o protocolo MAC pode variar conforme a tecnologia empregada. Com base nesse cenário

### assinale a alternativa correta sobre switches e arquiteturas de redes:

```txt
## R : Switches operam na camada 2 e utilizam endereços MAC para encaminhar quadros de forma eficiente.

### Entendimento : Switch's tambem operam na camada 2 (enlance) e usam MAC's para encaminhar dados (evitando colisões), Diferente de hubs replicam os dados para todas as portas, switches filtram e encaminham os quadros apenas para o destinatário correto.
```
---------------------------------------------------------------------------------------------------------------------------

## 5. Em uma empresa de médio porte, a equipe de TI está modernizando sua infraestrutura de rede para melhorar o desempenho da comunicação entre os dispositivos. Durante uma reunião, o administrador de redes explica que os switches desempenham um papel essencial na rede, pois encaminham quadros apenas para o destino correto, ao contrário dos antigos hubs, que replicavam o tráfego para todas as portas. Com base nesse cenário 

### assinale a alternativa correta sobre switches:

```txt
## R : Switches operam na camada 2 do modelo OSI, aprendendo endereços MAC e encaminhando quadros de forma eficiente.

### Entedimento :  Switichs oprem na 2° camada usando endereço MAC para evitar Congestionamento e garantia de entrega

```
---------------------------------------------------------------------------------------------------------------------------

## 6. Uma empresa está expandindo sua rede local e decidiu substituir seus antigos hubs por switches para melhorar o desempenho da comunicação. Durante a configuração, um técnico explica que os switches operam na camada 2 do modelo OSI e utilizam uma tabela interna para mapear endereços MAC às portas, permitindo transmissões simultâneas e comunicação full-duplex, o que dobra a largura de banda disponível para cada dispositivo. Com base nesse cenário

### assinale a alternativa correta sobre o funcionamento dos switches:

```txt
## R :  Switches permitem comunicação full-duplex, o que possibilita a transmissão e recepção de dados simultaneamente, dobrando a largura de banda.

### Entendimento : Switchs mais atuais (NOVOS) usam FULL-DUPLEX .
```
---------------------------------------------------------------------------------------------------------------------------

## 7. Durante a configuração de uma nova rede corporativa, um administrador de redes explica como os switches aprendem e gerenciam os endereços MAC dos dispositivos conectados. Ele menciona que, quando um switch recebe um quadro destinado a um endereço MAC desconhecido, ele realiza um processo chamado flooding, enviando o quadro para todas as portas, exceto a de origem. Com o tempo, o switch aprende os endereços e reduz esse tipo de tráfego desnecessário, otimizando a comunicação na rede. Com base nesse cenário

### assinale a alternativa correta sobre o aprendizado e inundação de MAC nos switches:

```txt
## R : Quando um switch não conhece o endereço MAC de destino, ele realiza flooding, enviando o quadro para todas as portas, exceto a de origem.

### Entendimento : pós receber uma resposta do dispositivo correto, o switch aprende o endereço MAC e atualiza sua tabela de comutação, evitando flooding futuro para aquele endereço.
Esse mecanismo otimiza a comunicação, reduz o tráfego desnecessário e melhora o desempenho da rede.
```
---------------------------------------------------------------------------------------------------------------------------

## 8. Uma empresa está substituindo seus antigos hubs por switches para melhorar a eficiência da rede. Durante o treinamento da equipe de TI, o administrador explica que hubs compartilham um único domínio de colisão, o que pode causar congestionamento na rede. Em contrapartida, switches criam um domínio de colisão separado para cada porta, permitindo transmissões simultâneas sem interferências, o que melhora significativamente o desempenho da rede. Com base nesse cenário

### assinale a alternativa correta sobre domínios de colisão:

```txt
## R : Switches criam domínios de colisão separados para cada porta, permitindo que múltiplos dispositivos transmitam simultaneamente sem interferências.

### Entendimento : Isso melhora significativamente o desempenho da rede, reduzindo colisões e permitindo comunicação full-duplex (transmissão e recepção simultânea).
Como resultado, switches são muito mais eficientes que hubs 
```
---------------------------------------------------------------------------------------------------------------------------

## 9. Uma empresa de médio porte está enfrentando problemas de congestionamento na rede devido ao alto volume de tráfego de broadcast. O administrador de redes explica que switches, por padrão, não segmentam domínios de broadcast, o que pode levar a sobrecarga da rede quando muitos dispositivos estão conectados. Para solucionar esse problema, ele propõe o uso de VLANs, que permitem dividir um único switch em redes lógicas separadas, melhorando a eficiência do tráfego.

### assinale a alternativa correta sobre domínios de broadcast e VLANs:

```txt
## R : Switches não dividem domínios de broadcast por padrão, mas VLANs permitem segmentar a rede logicamente.

### Entendimento : VLANs permitem dividir um único switch em múltiplos domínios de broadcast lógicos, criando redes independentes dentro do mesmo equipamento.
Além disso, VLANs aumentam a segurança e a organização da rede, permitindo isolar diferentes departamentos ou tipos de tráfego.
```
---------------------------------------------------------------------------------------------------------------------------

## 10. Uma grande empresa está reestruturando sua rede para melhorar a comunicação entre diferentes setores. O administrador de redes sugere o uso de switches de Camada 3, que combinam as funcionalidades de um switch tradicional com capacidades de roteamento. Ele explica que esses dispositivos analisam endereços IP além de MAC, permitindo a comunicação entre VLANs sem a necessidade de um roteador dedicado, além de suportarem protocolos como RIP e OSPF para otimizar o tráfego de rede. 

### Com base nesse cenário, assinale a alternativa correta sobre switches de Camada 3:
```txt
## R : Switches de Camada 3 permitem comunicação entre VLANs e utilizam protocolos de roteamento como RIP e OSPF.

### Entendimento : Diferente dos switches tradicionais, que operam apenas com endereços MAC, os switches de Camada 3 são capazes de tomar decisões baseadas em endereços IP, funcionando de forma similar a um roteador.
```
---------------------------------------------------------------------------------------------------------------------------
# LEMBRETE OSPF e RIP :

### RIP = "Roteador Ingênuo e Preguiçoso"
### Se a empresa tem uma rede simples e pequena, RIP pode ser suficiente. Mas para qualquer coisa maior ou que precise de desempenho e segurança, OSPF é a melhor escolha.

### OSPF = "Organizado, Sofisticado, Profissional e Ferido de guerra"
### Se a empresa crescer, RIP pode virar um problema por conta da limitação de saltos e lentidão, enquanto OSPF já está preparado para expansão.


```lua
                          +-----------------------------+
                          |        ROTEADOR (Camada 3)  |
                          |  - Usa RIP / OSPF           |
                          |  - Roteia entre redes/VLANs |
                          +--------------+--------------+
                                         |
                                  (Roteamento IP)
                                         |
                  +----------------------+--------------------+
                  |                                           |
     +------------v------------+               +-------------v------------+
     |   SWITCH CAMADA 3       |               |   SWITCH CAMADA 2        |
     | - Divide VLANs          |               | - Divide VLANs           |
     | - Pode usar RIP/OSPF ✅ |               | - NÃO usa RIP/OSPF ❌   |
     | - Faz roteamento L3     |               | - Trabalha com MAC       |
     +------------+------------+               +-------------+------------+
                  |                                           |
          +-------+---------+                          +------+-------+
          |      VLAN 10    |                          |     VLAN 20  |
          | (Ex: Financeiro)|                          |  (Ex: RH)    |
          +-----------------+                          +--------------+


```
---------------------------------------------------------------------------------------------------------------------------
## 11. Uma empresa está adquirindo novos switches para otimizar o desempenho da rede e minimizar a latência na transmissão de dados. Durante a seleção do equipamento, o administrador de redes explica que os switches utilizam diferentes métodos de comutação para encaminhar quadros de dados. O método store-and-forward verifica erros antes de encaminhar os quadros, enquanto o cut-through permite um encaminhamento mais rápido, transmitindo os dados assim que identifica o endereço MAC de destino. Já o método fragment-free aguarda os primeiros 64 bytes antes de encaminhar o quadro, equilibrando velocidade e confiabilidade. Com base nesse cenário. 

### assinale a alternativa correta sobre os métodos de comutação:
```txt
## R : O método store-and-forward verifica a integridade do quadro antes de encaminhá-lo, garantindo maior confiabilidade.

## Entendimento :
Store-and-Forward: Armazena todo o quadro, verifica erros e depois encaminha.

Cut-Through: Encaminha o quadro assim que le o endereço MAC de destino.

Fragment-Free: Aguarda os 64 primeiros bytes para evitar colisões antes de encaminhar.
```
---------------------------------------------------------------------------------------------------------------------------
```md


📶 Camada 2 – Enlace de Dados (Data Link Layer)
Atua diretamente com o endereçamento MAC.

Responsável pela comunicação direta entre dispositivos em uma mesma rede local (LAN).

Define como os dados são empacotados em quadros (frames).

Dispositivos típicos: Switches, Bridges.

Faz detecção de erros e controle de fluxo.

Switches operam aqui (aprendem MACs e encaminham frames corretamente).



🌐 Camada 3 – Rede (Network Layer)
Responsável pelo endereçamento lógico (IP) e roteamento.

Determina o melhor caminho para os dados irem de uma rede a outra.

Trabalha com pacotes (packets).

Dispositivos típicos: Roteadores, Switches de Camada 3.

Protocolos: IP, ICMP, ARP, RIP, OSPF, BGP.



🔌 Switches
Dispositivo de camada 2 (e também camada 3, nos modelos avançados).

Aprende os endereços MAC e encaminha dados somente para a porta correta.

Permite comunicação full-duplex (transmissão e recepção simultâneas).

Cada porta de um switch = domínio de colisão separado.

Reduz colisões, melhora desempenho.



🌎 Roteadores
Dispositivos de camada 3.

Conectam redes diferentes e escolhem o melhor caminho para pacotes.

Usam endereços IP e tabelas de roteamento.

Podem rodar protocolos de roteamento dinâmico como RIP, OSPF, BGP.



🧱 VLANs (Virtual LANs)
Criam redes lógicas separadas dentro de um mesmo switch físico.

Permitem segmentar domínios de broadcast.

Melhoram segurança, controle de tráfego e organização da rede.

Para comunicação entre VLANs, é necessário roteamento (Inter-VLAN Routing), feito por roteadores ou switches de camada 3.



✉️ Pacotes
Unidade de dados na Camada 3 (rede).

Contêm:

Endereço IP de origem e destino

Dados de controle

Dados a serem entregues

São encapsulados em quadros (Camada 2) para transmissão física.



📡 RIP (Routing Information Protocol)
Protocolo de roteamento interno (IGP).

Usa distância (número de saltos) como métrica para escolher o caminho.

Limite de 15 saltos → redes maiores que isso não são alcançáveis.

Atualiza a tabela de roteamento a cada 30 segundos (pode causar lentidão).

Simples, mas pouco escalável. Usado em redes menores ou para fins educacionais.

Versões:

RIP v1: Não suporta CIDR nem VLSM.

RIP v2: Suporta sub-redes, VLSM, e autenticação.



🌍 BGP (Border Gateway Protocol)
Protocolo de roteamento entre sistemas autônomos (EGP).

Usado para conectar grandes redes, como as da Internet.

Trabalha com endereços IP e políticas.

Usa o conceito de AS (Autonomous Systems).

Suporta RIP e OSPF internamente, mas BGP para o mundo exterior.

Robusto e altamente configurável.

```
-------------------------------------------------------------
```md

✅ Seu conhecimento até agora – avaliação:
O que você mandou:
VLANs na Camada 2 ✔️

Separam um switch físico em redes lógicas ✔️

Reduzem tráfego de broadcast ✔️

Switches de Camada 3 existem e usam BGP, RIP, OSPF ✔️

RIP limitado a 15 saltos, bom pra redes pequenas ✔️

OSPF é mais seguro e usado em redes grandes ✔️

BGP trabalha junto com os dois (mais ou menos, vamos falar disso também) ➖

Nota: você tá bem no caminho! Mas agora, bora refinar os pontos sobre Switches de Camada 2, como pediu


🎛️ Switches de Camada 2 – o que você precisa saber
📍 Operam na Camada 2 (Enlace de Dados) do modelo OSI:
Usam endereços MAC para encaminhar quadros.

São responsáveis por comutação (switching) local — ou seja, conectam dispositivos dentro da mesma rede (LAN).



🧠 Principais funções:
Aprendizagem de MAC: ele escuta quem está em qual porta e armazena isso na tabela MAC.

Encaminhamento: envia quadros apenas pra porta correta (com base no MAC de destino).

Filtragem: bloqueia envio desnecessário de pacotes pra todas as portas (diferente de um hub).

Domínio de colisão separado por porta: cada porta é um domínio de colisão isolado, ou seja, não tem interferência como no hub.

Mas compartilham o mesmo domínio de broadcast — a menos que você use VLANs.




🔌 Switches + VLANs:
VLANs permitem ao switch de Camada 2 criar vários domínios de broadcast separados.

Mesmo sendo Camada 2, ele consegue separar redes logicamente, mas não faz roteamento entre elas por conta própria.

Pra VLANs se comunicarem entre si, é necessário:

Um roteador externo (Roteamento entre VLANs)

Ou um switch de Camada 3, que já tem a capacidade de roteamento interno.




⚙️ Switches de Camada 3 – só pra comparar
Operam na Camada 2 E 3 do modelo OSI.

Fazem roteamento entre VLANs, ou seja, conseguem falar entre redes separadas.

Podem rodar protocolos de roteamento dinâmico como:

RIP (simples, 15 saltos)

OSPF (avançado, para empresas)

BGP (usado pra interligar grandes redes, como provedores e sistemas autônomos)

🚨 Obs:
BGP não “suporta” o RIP ou OSPF — ele atua em outro nível, conectando redes inteiras.

É mais comum em roteadores e switches de backbone (provedores, datacenters).




⚡Resumo prático do que falta sobre switches Camada 2:

Conceito	Camada 2 (Switch Básico)
Roteia IPs?	                  ❌ Não
Encaminha por MAC?	          ✔️ Sim
Usa VLAN?                    	✔️ Sim
Separa domínio de colisão?	  ✔️ Por porta
Separa domínio de broadcast?	❌ Só com VLAN
Usa RIP/OSPF/BGP?	            ❌ Não (isso é Camada 3)
Tráfego entre VLANs?        	❌ Precisa de Camada 3

```
