# Tecnicas Digitales G3-E2

Técnicas Digitales - Grupo 3 Equipo 2

## Descripción
Este es el repositorio de la asignatura tecnicas digitales.

## Integrantes

* Ivan Eduardo Beltran Prieto
(https://github.com/ivanedbeltranpr-star)
* Cristian Camilo Romero Contreras
(https://github.com/cristiancaromeroco-dotcom)
* Sebastian Ferney Gutierrez Mondragón
(https://github.com/sebastianfegutierrezmo-ops)

# Informe

Indice:

1. [Contador](#sumador-de-3-bits)
2. [Simulaciones](#simulaciones)
3. [Evidencias de implementación](#evidencias-de-implementación)
4. [Conclusiones](#conclusiones)


## Documentación del diseño implementado

## 1. Contador

#### 1.1 Descripción

• Módulo Principal (contador_digital.v):
Se encarga de la decodificación de datos. Utiliza bloques combinacionales always y estructuras case para traducir los valores numéricos binarios a un vector de 7 bits. La asignación física hacia la FPGA se realiza mediante la instrucción assign. El display opera bajo la configuración de ánodo común (lógica inversa), donde un 0 lógico enciende el segmento y un 1 lo apaga.
• Banco de Pruebas (contador_digital_tb.v):
Es un entorno de simulación no sintetizable (testbench) creado para verificar el funcionamiento del circuito. Define las entradas como reg para controlar sus estados y las salidas como wire. Instancia el módulo principal como UUT (Unidad Bajo Prueba), genera una señal de reloj periódica invirtiendo su estado cada 9 unidades de tiempo y utiliza un bloque initial para aplicar los estímulos de reinicio y conteo.




