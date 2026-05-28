# Calculadora_Cient-fica
La Calculadora Científica Graficadora es un programa interactivo desarrollado en Python que permite realizar operaciones matemáticas avanzadas directamente desde la terminal, sin necesidad de instalar librerías externas. Todas las funciones matemáticas están implementadas desde cero mediante algoritmos propios.
Características principales:
Interfaz de menú interactiva en consola.
Operaciones básicas y científicas con alta precisión.
Funciones trigonométricas, hiperbólicas e inversas.
Graficador ASCII para visualizar funciones en el rango deseado.
Historial automático de todas las operaciones realizadas.
Sin dependencias externas: corre con Python estándar.

4. Menú principal
Al ejecutar el programa verá el siguiente menú. Escriba el número de la opción deseada y presione Enter.


5. Operaciones básicas (Opción 1)
Acceda escribiendo 1 en el menú principal. Se mostrará un submenú con 7 operaciones:

Suma, Resta, Multiplicación, División, Potencia, Módulo:
Ingrese el primer número cuando el programa lo solicite, luego el segundo. El resultado se muestra inmediatamente y se guarda en el historial.

Raíz n-ésima:
Ingrese el número al que se le calculará la raíz y el índice n. Ejemplo: raíz cúbica de 27 → número: 27, índice: 3, resultado: 3.

Restricciones importantes:
No se puede dividir entre cero.
No se puede calcular el módulo con divisor cero.
La raíz de índice par de un número negativo no es real.

6. Operaciones científicas (Opción 2)
Incluye 9 funciones avanzadas. Seleccione el número correspondiente e ingrese el valor de x:


7. Trigonometría (Opción 3)
Todas las funciones trabajan en radianes. Si tiene ángulos en grados, use primero la conversión (opciones 7 y 8).

sin(x), cos(x), tan(x): calculan las funciones trigonométricas básicas.
arcsin(x), arccos(x), arctan(x): funciones inversas. arcsin y arccos requieren −1 ≤ x ≤ 1.
Convertir grados a radianes: ingrese el ángulo en grados y obtiene el equivalente en radianes.
Convertir radianes a grados: operación inversa.

Nota: la tangente no está definida en π/2 + k·π (aproximadamente ±1.5708, ±4.7124…).

8. Combinatoria (Opción 4)
Permite calcular combinaciones y permutaciones. En ambos casos se solicitarán los valores n y r (enteros positivos con r ≤ n).

Combinaciones C(n, r) = n! / (r! × (n−r)!) — orden no importa.
Permutaciones P(n, r) = n! / (n−r)! — orden sí importa.

Ejemplo — C(5, 2): n = 5, r = 2 → resultado: 10.

9. Evaluar una función (Opción 5)
Calcula el valor numérico de cualquiera de las 12 funciones predefinidas en un punto x específico.

Pasos:
Seleccionar la función por su número (1 al 12).
Ingresar el valor de x.
El programa muestra f(x) con 6 decimales de precisión.

Funciones disponibles:


10. Graficar una función (Opción 6)
Genera un gráfico ASCII de la función seleccionada en el rango horizontal indicado.

Pasos:
Seleccionar la función por su número (1 al 12).
Ingresar x mínimo (ej.: −5).
Ingresar x máximo (ej.: 5). Debe ser mayor que x mínimo.

Cómo interpretar el gráfico:
Los asteriscos (*) representan los puntos de la función.
El eje horizontal se marca con guiones (−) y el vertical con barras (|).
La intersección de los ejes se indica con el símbolo (+).
Los valores de y se muestran a la izquierda (máximo, medio, mínimo).
Los valores de x se muestran debajo (mínimo, medio, máximo).

Recomendaciones de rango por función:
Seno / Coseno / Tangente: [−6.28, 6.28] (dos períodos completos).
Exponencial: [−3, 3] (crece rápidamente para x grande).
Logaritmo: [0.1, 10] (no existe para x ≤ 0).
Funciones polinomiales: [−5, 5] como punto de partida.

11. Historial (Opción 7)
El historial registra automáticamente cada operación realizada durante la sesión actual. Al seleccionar esta opción se muestran todas las operaciones numeradas.

El historial se mantiene mientras el programa esté en ejecución.
Al cerrar el programa el historial se pierde (no se guarda en disco).
Puede borrar el historial en cualquier momento respondiendo 's' cuando se pregunte.

12. Manejo de errores
El programa valida las entradas y muestra mensajes descriptivos cuando se produce un error, sin interrumpir la ejecución. Los errores más comunes son:


