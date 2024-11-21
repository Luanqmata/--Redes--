# Questões de Redes e Protocolos

1. **O que significa arquitetura TCP/IP? Explique.**

2. **O protocolo UDP é baseado em sessão? Justifique.**  
   **R:** Protocolo UDP: Não é baseado em sessão. Ele oferece um serviço de datagrama, ou seja, cada pacote é enviado independentemente, sem garantia de entrega na ordem correta ou livre de duplicação.

3. **Em qual camada o protocolo IP opera?**  
   **R:** Camada de rede. O IP é o protocolo principal da camada de rede, responsável por endereçar e rotear pacotes entre redes.

4. **Qual é a porta padrão para HTTPS?**  
   **R:** Porta 443.

5. **O protocolo DHCP tem a função de controlar o fluxo de dados. Justifique se a afirmação anterior é Verdadeira ou Falsa.**  
   **R:** Falso. O DHCP atribui endereços IP e outros parâmetros de configuração a dispositivos em uma rede, mas não controla o fluxo de dados.

6. **Explique a principal função do DNS.**  
   **R:** DNS (Domain Name System): Traduz nomes de domínio legíveis (como www.exemplo.com) em endereços IP numéricos, facilitando a localização de dispositivos na internet.

7. **“A camada de transporte do modelo TCP/IP lida com...” Desenvolva.**  
   **R:** A camada de transporte do modelo TCP/IP lida com: A comunicação end-to-end entre processos em hosts diferentes. Protocolos como TCP (garante a entrega confiável) e UDP (entrega não confiável) operam nessa camada.

8. **Qual protocolo é responsável por fornecer endereços IP dinâmico?**  
   **R:** DHCP.

9. **“A função do ICMP é transferir dados criptografados”, Discorra sobre essa afirmação.**  
   **R:** Falsa. O ICMP é usado para enviar mensagens de controle e diagnóstico, como ping, traceroute e mensagens de erro, não para transferir dados criptografados.

10. **No TCP/IP qual a função do IP de LoopBack?**  
    **R:** IP de Loopback: Serve para testes locais, permitindo que um dispositivo se comunique consigo mesmo. O endereço mais comum é 127.0.0.1.

11. **Qual a função do ARP?**  
    **R:** ARP: Mapeia endereços IP em endereços MAC para permitir a comunicação local em uma rede.

12. **Qual protocolo é usado para transferência de arquivos?**  
    **R:** FTP (File Transfer Protocol), SFTP (SSH File Transfer Protocol), TFTP (Trivial File Transfer Protocol) e outros.

13. **O que é o protocolo SMTP, sua função e o socket no LoopBack.**  
    **R:** SMTP (Simple Mail Transfer Protocol): É usado para enviar e-mails.

14. **“A camada de aplicação no modelo TCP/IP inclui os protocolos HTTP e FTP.” Justifique ou corrija explicando essa afirmação.**  
    **R:** Verdadeiro. HTTP e FTP são exemplos de protocolos de aplicação, operando na camada mais alta do modelo TCP/IP.

15. **Qual o significado de TTL e qual a sua função?**  
    **R:** TTL: É um campo no cabeçalho do pacote IP que indica o número máximo de saltos que um pacote pode fazer antes de ser descartado.

16. **Qual serviço roda na porta 443 e qual a sua principal diferença para o protocolo da porta 80?**  
    **R:** Porta 443 = HTTPS, Porta 80 = HTTP. A diferença principal é a segurança por meio de criptografia.

17. **Qual o protocolo utilizado para enviar emails?**  
    **R:** SMTP.

18. **Explique o que é, o que significa e qual a função do NAT?**  
    **R:** NAT: É uma técnica que permite que várias redes internas compartilhem um único endereço IP público, economizando endereços e facilitando a gestão de redes.

19. **Qual a função do Gateway?**  
    **R:** Gateway: É um dispositivo que conecta duas redes diferentes, traduzindo protocolos e formatando dados para permitir a comunicação entre elas.

20. **Qual camada do modelo TCP/IP é responsável pelo roteamento de pacotes?**  
    **R:** Camada de rede.

21. **Qual camada está o protocolo SNMP? Explique sua função.**  
    **R:** Camada de gerenciamento de rede. O SNMP é usado para monitorar e gerenciar dispositivos em uma rede.

22. **Qual o papel do endereço MAC?**  
    **R:** Endereço MAC: Identifica de forma única uma interface de rede em um dispositivo. É usado para comunicação local em uma rede.

23. **Qual o protocolo é usado para resolver nomes de domínio?**  
    **R:** DNS (Domain Name System).

24. **Qual a função do POP3? Explique.**  
    **R:** POP3 (Post Office Protocol version 3): É um protocolo de recebimento de e-mails, permitindo que os clientes baixem e-mails de um servidor de correio.

25. **Quais protocolos são responsáveis pela criptografia de E-Mails?**  
    **R:** SMTP (com TLS/SSL), IMAP (com SSL), POP3 (com SSL).

26. **O protocolo HTTP opera em qual camada?**  
    **R:** Camada de aplicação.

27. **Que protocolo opera por Default no socket 192.168.1.100:23?**  
    **R:** Telnet.

28. **Qual é o papel do protocolo RIP?**  
    **R:** RIP (Routing Information Protocol): É um protocolo de roteamento dinâmico simples, utilizado para trocar informações sobre rotas entre roteadores em uma rede.

29. **“O protocolo IGMP é utilizado para...” Desenvolva.**  
    **R:** Gerenciar a associação de hosts a grupos multicast, permitindo que um único pacote seja enviado para múltiplos destinatários simultaneamente.

30. **O que é endereço de BroadCast?**  
    **R:** Endereço de Broadcast: É um endereço especial que permite enviar um pacote para todos os dispositivos em uma rede.

31. **Qual é o protocolo responsável pela transferência de Hyper-Text?**  
    **R:** HTTP (Hypertext Transfer Protocol).

32. **Qual é a máscara de uma sub-rede classe C?**  
    **R:** 255.255.255.0.

33. **Qual a função do SSH? Justifique.**  
    **R:** SSH: Permite a conexão segura e remota a outros computadores, garantindo a confidencialidade, integridade e autenticidade dos dados transmitidos.

34. **Qual o protocolo responsável pelo envio de mensagens ICMP?**  
    **R:** IP.

35. **Qual é a principal função do IPv6?**  
    **R:** Oferece um espaço de endereçamento muito maior que o IPv4, resolvendo o problema da escassez de endereços IP.

36. **Qual protocolo é utilizado para obter informações sobre a topologia da rede?**  
    **R:** SNMP.

37. **No TCP/IP a tradução de nomes de domínio em endereços IP é feita por qual protocolo?**  
    **R:** DNS.

38. **Qual a função do protocolo BGP? Explique.**  
    **R:** BGP (Border Gateway Protocol): É um protocolo de roteamento dinâmico utilizado para trocar informações sobre rotas entre redes autônomas na internet.

39. **Descreva o protocolo SMTP.**  
    **R:** SMTP (Simple Mail Transfer Protocol): É um protocolo de envio de e-mails, responsável por transferir mensagens entre servidores de correio.

40. **O IPv4 é caracterizado por um endereçamento de 128 bits? Justifique a sua resposta.**  
    **R:** Falso. O IPv4 é caracterizado por um endereçamento de 32 bits, enquanto o IPv6 utiliza um endereçamento de 128 bits.
