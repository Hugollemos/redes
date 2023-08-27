O IPv4 é formado por 32 bits divididos em 4 octetos (8 bits cada). Eles são representados por números de 0 a 255, tal como 192.168.100.2, por exemplo. Além disso, o IPv4 precisa de algo chamado de máscara de sub-rede, que trata de definir qual parte do IP representa a rede e qual parte representa os hosts daquela rede.
Ex:
```
192.168.100.2
255.255.255.0
```
O cálculo do endereço IPv4 envolve a conversão de um endereço IP decimal em um formato binário e vice-versa. O IPv4 é um sistema de endereçamento de 32 bits, dividido em quatro octetos (8 bits cada), separados por pontos. Cada octeto pode ter um valor entre 0 e 255.

Para entender o cálculo do IPv4, vamos considerar o seguinte exemplo: 192.168.0.1

1. Conversão decimal para binário:
   - Converta cada octeto decimal em seu equivalente binário. No nosso exemplo:
     - 192 em binário é 11000000
     - 168 em binário é 10101000
     - 0 em binário é 00000000
     - 1 em binário é 00000001

   Portanto, o endereço IPv4 192.168.0.1 em binário é: 11000000.10101000.00000000.00000001

2. Conversão binário para decimal:
   - Converta cada octeto binário em seu equivalente decimal. No nosso exemplo:
     - 11000000 em decimal é 192
     - 10101000 em decimal é 168
     - 00000000 em decimal é 0
     - 00000001 em decimal é 1

   Portanto, o endereço IPv4 11000000.10101000.00000000.00000001 em decimal é: 192.168.0.1

Além disso, o endereço IPv4 também pode ser dividido em duas partes: endereço de rede e endereço de host. A divisão entre essas partes é determinada pela máscara de sub-rede.

A máscara de sub-rede é usada para determinar quais bits no endereço IP pertencem à parte da rede e quais bits pertencem à parte do host. A máscara de sub-rede é representada por uma sequência de 1s seguidos de 0s. Por exemplo, uma máscara de sub-rede típica é 255.255.255.0, que em binário é 11111111.11111111.11111111.00000000.

Para calcular a rede e o host de um endereço IPv4 usando uma máscara de sub-rede, você faz uma operação chamada AND lógico bit a bit entre o endereço IP e a máscara de sub-rede.

Por exemplo, se tivermos o endereço IP 192.168.0.1 e a máscara de sub-rede 255.255.255.0, faremos a seguinte operação AND:

- 192.168.0.1 (binário: 11000000.10101000.00000000.00000001)
- 255.255.255.0 (binário: 11111111.11111111.11111111.00000000)

Realizando a operação AND bit a bit, obtemos:

11000000.10101000.00000000.00000001 AND
11111111.11111111.11111111.00000000
-------------------------------------
11000000.10101000.00000000.00000000

Portanto, a parte da rede é 192.168.0.0 e a parte do host é 0.0.0.1.

Espero que isso esclareça o funcionamento do c

álculo do IPv4!

https://www.todoespacoonline.com/w/2015/06/calculo-de-sub-redes-ipv4/#:~:text=O%20IPv4%20é%20formado%20por,representa%20os%20hosts%20daquela%20rede.