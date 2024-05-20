USART


**Registry to controle the Status and the Data (UCSR0A and UCSR0B)** :

* These registers controle USART configurations, how to enable the transmission and reception of data
* Bit TXEN and RXEN0 are used to enable transmission and reception respectivvely.


![](assets/20240222_014937_image.png)

**Registro de Configuração de Modo (UCSR0C)** :

* Este registro determina o modo de operação da USART, como o modo assíncrono ou síncrono, número de bits de dados, paridade, e número de bits de parada.


**Registros de Baud Rate (UBRR0H e UBRR0L)** :

Esses registros determinam a velocidade de comunicação, ou baud rate, configurando o valor do divisor de clock.
O valor do divisor de clock é calculado usando a fórmula:

$$ UBRR= { {ClockRequency \over 16 * BaudRate} - 1 }$$

Assumindo a frequência de clock típica do microcontrolador de 16MHz ($16*10^6$) e o baudrate de $9600$, calculamos o UBRR da seguinte forma:

$$ UBRR= { {16*10^2 \over 16 * 9600} - 1 = 113,1667}$$





Links Úteis:
[The Ultimate Guide to Arduino Nano Pinout](https://www.nextpcb.com/blog/arduino-nano-pinout)
[AVR Libc Home Page - Special function register](https://www.ele.uva.es/~jesus/perifericos/avr-libc-user-manual-1.4.5/group__avr__sfr.html)
[HC-05 Bluetooth Module Interfacing with AVR ATmega16/ATmega32](https://www.electronicwings.com/avr-atmega/hc-05-bluetooth-module-interfacing-with-atmega1632)
[Arduino Nano Pinout, Projects & Spec](https://devboards.info/boards/arduino-nano)
[Playing with Arduino - Serial Communication Registre](https://garretlab.web.fc2.com/en/arduino/inside/hardware/arduino/avr/cores/arduino/HardwareSerial.cpp/registers.html)
[USART / UART Register Description : Arduino / ATmega328p](https://www.arnabkumardas.com/arduino-tutorial/usart-register-description/)
