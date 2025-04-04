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
## 11.
