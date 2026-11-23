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

1. [Contador](#Semaforo)
2. [Simulaciones](#simulaciones)
3. [Evidencias de implementación](#evidencias-de-implementación)
4. [Conclusiones](#conclusiones)


## Documentación del diseño implementado

## 1. Semaforo 

#### 1.1 Descripción

El diseño consiste en la programación en Verilog de una máquina de estados finitos (FSM) que simula el funcionamiento de un semáforo. El sistema controla de manera secuencial y temporizada la transición entre sus tres luces principales: inicia en rojo (detención), cambia a naranja (precaución/transición) y finalmente pasa a verde (avance), asegurando un ciclo lógico, ordenado y sincronizado mediante señales de reloj.

![Descripción de la imagen](img/sem.jpg)  
![Descripción de la imagen](img/sema.jpg)

## Simulaciones

### Simulación Contador

La siguiente imagen muestra la simulación temporal en GTKWave del controlador de semáforo vehicular y peatonal desarrollado en Verilog. En el diagrama de ondas se verifica la sincronización del sistema frente a las señales de reloj y reinicio, evidenciando la conmutación ordenada y mutuamente excluyente entre las luces vehiculares (rojo, amarillo y verde) y su correcta correspondencia con el paso peatonal (peaton_rojo y peaton_verde), garantizando así la seguridad y el cumplimiento lógico de cada estado.

![Descripción de la imagen](imagen3a/sem.jpg)  

## Evidencias De La Implementación

(https://youtu.be/NPtj6FsX_fE)

## Conclusiones






