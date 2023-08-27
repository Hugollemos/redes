## TPC/IP é um conjunto de protocolos de comunicação.

| TCP/IP | OSI |
| --- | --- |
| Aplicação | Aplicação, Apresentação, Sessão |
| Transporte | Transporte|
| Rede(Internet) | Rede |
| Física | Enlace, Física |

| TCP/IP | EXEMPLOS |
| --- | --- |
| Aplicação | HTTP, SMTP, IMAPV.4 FTP, SIP, SSH, TELNET |
| Transporte | TCP/UDP|
| Rede(Internet) | IPV4, IPV6 |
| Física | ARP, ETHERNET, FDDI |

## IP é o endereço lógico que cada equipamento tem na rede.
 
- classes de IP.
    - A - 0 a 127 -> 16.777.214 equipamentos,
primeiro número indentifica a REDE o outros 3 o HOTS. 10.1.1.10
    - B - 128 a 191 -> 65.536 equipamentos,
Os dois primeiros identificam a REDE e outros 2 o HOST. 172.16.10.1
    - C - 192 a 223 -> 254 equipamentos,
Os 3 primeiros identificam a REDE e o último o ROST. 192.168.0.1
    - D - 224 a 239 -> Reservado para Multicast, unicast, broadcast, anycast.
    - E - 240 a 55 -> Reserva para teste de novas tecnologias

---

## Máscara de rede é um termo usado em redes de computadores para definir a classe e o intervalo de endereços IP (Internet Protocol).

```bash
Máscara de rede de classe
A: 255.0.0.0
B: 255.255.0.0
c: 255.255.255.0
```
--- 
- servidor DHCP (Dynamic Host Configuration Protocol) a função dele é fazer as máquinas de determinada rede consigam obter o endereçamento IP de maneira automática. 
- endereço IP;
- gateway padrão;
- máscara de sub-rede;
- entre outras configurações.

# APIPA
Automatic Private IP Addressing / Endereçamento IP privado automático
- endereço de configuração automática do windows
- Atribui automaticamente IP a uma estação caso haja falha na comunicação
- Garante a comunicação entre as estaçoes dentro de uma rede local

# Faixa de Endereços do APIPA
Há uma faixa de endereços reservados pelo IETF que são atribu;iveis por meio do APIPA