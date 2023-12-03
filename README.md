# Programa-7.-Paginaci-n-simple
## Requerimientos

1. **Algoritmo de Planificación:**
   - RR (Round-Robin) según la Actividad 10.

2. **Cumplir con los Requerimientos del Programa 5 (Actividad 10).**

3. **Asignación Aleatoria de Procesos:**
   - Tiempo, operación y tamaño asignados aleatoriamente (número aleatorio entero entre 6 y 26).

4. **Configuración de la Memoria:**
   - Capacidad de la memoria: 220.
   - División en "Marcos" de igual longitud (44 marcos de 5 cada uno).
   - 4 marcos ocupados por el S.O., quedando 40 disponibles para los procesos.
   - Procesos divididos en páginas (tamaño 5).

5. **Teclas a Utilizar:**

   | Tecla | ¿Qué Indica?                             | ¿Qué Hace?                                                  |
   |-------|------------------------------------------|------------------------------------------------------------|
   | I     | Interrupción por Entrada/Salida          | Proceso en ejecución sale del procesador y va a la cola de Bloqueados. Vuelve a la cola de listos después de un tiempo de 8. |
   | E     | Error                                    | Proceso en ejecución termina por error, se muestra en procesos terminados. Se libera espacio en memoria. |
   | P     | Pausa                                    | Detiene la ejecución momentáneamente, se reanuda con la tecla "C". |
   | C     | Continuar                                | Reanuda el programa pausado previamente con "P".            |
   | N     | Nuevo                                    | Genera un nuevo proceso con datos aleatorios. Planificador a largo plazo define su ingreso al sistema. |
   | B     | Tabla de Procesos (BCP de cada proceso) | Pausa el programa y muestra la tabla de procesos (BCP). Tecla "C" continúa la simulación en el punto donde quedó. |
   | T     | Tabla de Páginas                         | Detiene la ejecución y muestra la tabla de páginas de cada proceso, además de los marcos libres. Continúa al presionar la tecla "C". |

6. **Visualización en Pantalla:**
   a. Memoria dividida en "Marcos", mostrando la ocupación proporcional y el número de cada marco.
   b. Número de procesos en la cola de nuevos:
      - Para el proceso próximo a ingresar a Listos, se muestra su ID y tamaño para visualizar cuántos marcos libres se necesitarán.
   c. Proceso en ejecución, mostrando todos sus datos.
   d. Contador que representa el Quantum.
   e. Lista de procesos terminados, marcando los que tuvieron error.
   f. Contador global.

7. **Tabla de Páginas:**
   - Muestra qué página está en cada marco (entrada por proceso).
   - Indica la relación de marcos libres.

8. **Fin del Programa:**
   - Se presiona la tecla "ESC".

9. **Datos al Finalizar:**
   - Todos los datos de cada proceso, incluida la tabla de páginas.

![image](https://github.com/KleoMaple/Programa-7.-Paginaci-n-simple/assets/88137469/4003da65-3f94-4dd0-88c3-f8ac80217e21)
En este ejemplo se observan los 44 Marcos, 
numerados de 0 a 43. Los marcos 40 a 43
están ocupados por el S.O. (denotado por el 
color negro), dejando del marco 0 al 39
disponibles para ser ocupados por los 
distintos procesos. Como se indicó se 
necesita ver si el marco esta libre (en este 
caso se denota por la ausencia de color), si 
está ocupado y el proceso está listo (se 
observa el bloque marcado como azul y de 
forma proporcional, indicando así que hay 
fragmentación interna), si está ocupado y el 
proceso está bloqueado se observa un color 
morado y si está ocupado y el proceso está en 
ejecución se observa por el color rojo

