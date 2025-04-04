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

