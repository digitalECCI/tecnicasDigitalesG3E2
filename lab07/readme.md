# Tecnicas Digitales G3-E2

Técnicas Digitales - Grupo 3 Equipo 2

## Descripción
Este es el repositorio de la asignatura tecnicas digitales.

## Informe Proyecto Final

## Integrantes

* Ivan Eduardo Beltran Prieto
(https://github.com/ivanedbeltranpr-star)
* Cristian Camilo Romero Contreras
(https://github.com/cristiancaromeroco-dotcom)
* Sebastian Ferney Gutierrez Mondragón
(https://github.com/sebastianfegutierrezmo-ops)

# Informe

Indice:

1. [Sumador de 3 bits](#sumador-de-3-bits)
2. [Display 7 segmentos](#Display-7-segmentos)
3. [Simulaciones](#simulaciones)
4. [Evidencias de implementación](#evidencias-de-implementación)
5. [Conclusiones](#conclusiones)

## Documentación del diseño implementado

## 1. Enlace de Comunicación Serial UART entre FPGA y PC

#### 1.1 Descripción

El laboratorio consiste en el diseño e implementación en Verilog de un enlace de comunicación serial bidireccional (UART) configurado a una velocidad de 9600 baudios (con reloj del sistema de 50 MHz), que permite el intercambio de datos en tiempo real entre una tarjeta FPGA y un computador mediante un conversor USB-TTL y la terminal PuTTY.
El funcionamiento del sistema se divide en dos etapas principales:

1. Recepción de datos (PC \(\rightarrow \) FPGA): Desde la consola de PuTTY se envía un valor numérico hacia la FPGA (a través de la línea GPIO_RX). El módulo procesa la trama serial recibida y refleja dicho número de manera visual encendiendo los LEDs correspondientes en la placa (LEDR[9:0]).

2. Transmisión de datos (FPGA \(\rightarrow \) PC): Mediante la activación manual de los interruptores físicos de la tarjeta (SW[9:0], que representan valores de 0 a 1023) y al presionar el botón de envío (KEY0), el sistema sincroniza las entradas para evitar rebotes o metaestabilidad, detecta el flanco de bajada y transmite el dato serialmente por el pin GPIO_TX, logrando que el número configurado en los pines aparezca directamente en la pantalla de PuTTY.





