USART


**Registry to controle the Status and the Data (UCSR0A and UCSR0B)** :

* These registers controle USART configurations, how to enable the transmission and reception of data
* Bit TXEN and RXEN0 are used to enable transmission and reception respectivvely.


![](assets/20240222_014937_image.png)

**Registro de Configuração de Modo (UCSR0C)** :

* Este registro determina o modo de operação da USART, como o modo assíncrono ou síncrono, número de bits de dados, paridade, e número de bits de parada.


**Registros de Baud Rate (UBRR0H e UBRR0L)** :

* Esses registros determinam a velocidade de comunicação, ou baud rate, configurando o valor do divisor de clock.
* O valor do divisor de clock é calculado usando a fórmula:
