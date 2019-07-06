# Apuntes de estadística

## Qué es la estadística?

Basada en tres disciplinas:
1. Análisis de datos: Recopilación, organización y resumen de los datos.
2. Probabilidad.
3. Inferencia estadística: Ciencia que extrae conclusiones a partir de datos concretos basándose en el cálculo de probabilidades.

## Estadística descriptiva

### Visualización

Para mostrar datos se pueden usar:

- Diagramas de puntos.
- Tablas de frecuencias.
- Tablas de frecuencias relativas.
- Histógrama.
- Histograma de frecuencias relativas.
- Gráfico de tallos y hojas.
- Gráfico de caja.

### Resumen numérico


| Observacion       | 1     | 2     | 3     | ... | n     |
| ----------------- | ----- | ----- | ----- | --- | ----- |
| Conjunto de datos | $x_1$ | $x_2$ | $x_3$ | ... | $x_n$ |

Indicadores simples de las características básicas de un conjunto de datos:

- Valor central.
  - Media.
  - Mediana. 
- Dispersión.
  - Recorrido intercuartílico.
  - Desviación estándar (o desviación típica).
 
#### Media

La media es el promedio de los datos.

$$\overline{x} = \sum_{i=1}^n \frac{x_i}{n}$$

#### Mediana.

Punto medio de datos obtenido después de ordenr los datos de menor a mayor. La mediana es el valor que queda al centro. Si el número de observaciones es par, la mediana será la media de los valores que quedan en el centro.

#### Recorrido intercuartílico

Dividir los datos ordenados numéricamente en cuatro grupos iguales y observar la distancia que separa los grupos extremos.

$$ IQR = Q_3 - Q_1 $$
Procedimiento de cálculo:

1. Ordenar datos numéricamente.
2. Dividir datos por la mediana ($Q_2$) en dos grupos iguales, si la mediana coincide con un dato, incluirlo en los dos grupos.
3. Calcular la mediana del grupo inferior. Ese será el primer cuartil, o $Q_1$.
4. Calcular la mediana del grupo superior. Ese será el tercer cuartil, o $Q_3$.

#### Desviación estándar

Distancia media entre los datos y la media $\overline{x}$

$$ s = \sqrt{\frac{1}{n-1} \sum_{i=1}^n{(x_i - \overline{x})^2}} $$

#### Puntaje Z

Número de desviaciones estándares que dista un punto de la media.

$$z_i = \frac{x_i-\overline{x}}{s}$$

### Propiedades de $\overline{x}$ y $s$

- 68% de los datos se encuentra a menos de una desviación estándar de la media.
- 95% de los datos se encuentra a menos de dos desviaciones estándares de la media.

## La probabilidad

### Definiciones básicas

- Experimiento aleatorio: Es el proceso de observa el resultado de un suceso casual. $O$
- Resultados elementales: Todos los posibles resultados del experimiento aleatorio. $O_1, O_2, ..., O_n$
- Espacio muestral: Conjunto o compendio de todos los resultados elementales.
- Probabilidad: Peso numérico asignado para medir la psobilidad de que un resultado se cumpla. $P(O_i)$
- Probabilidad condicionada: Probabilidad de que ocurra un suceso A sabiendo que el suceso B ya ha ocurrido. $P(a|B)$
- Independencia de sucesos: Dos sucesos son independientes si la aparición de uno no influye en la probabilidad del otro.

### Propiedades

1. Las probabilidades nunca son negativas. 

$$P(O_i) \geq 0$$

2. Si un suceso es seguro, le asignamos un valor de 1. Por lo tanto, la probabilidad total del espacio muestral debe ser 1.

$$P(O_1) + P(O_2) + ... + P(O_i)=1$$

3. Suma

$$P(A \cup B)= P(A)+P(B)+P(A \cap B)$$

4. Suma, cuando ambos sucesos son mutuamente excluyentes.

$$P(A \cup B)= P(A)+P(B)$$

5. Resta

$$P(A)=  1 - P(\overline{A})$$

6. Multiplicación

$$P(A \cap B)= P(A|B)P(B)$$

7. Condición

$$P(A | B)= \frac{P(A \cap B)}{P(B)} $$

8. En sucesos independientes A y B.

$$P(A) = P(A|B)$$

9. Multiplicación en sucesos independientes

$$P(A \cap B)= P(A)P(B)$$

### Teorema de Bayes

$$P(A|B) = \frac{P(A)P(B|A)}{P(A)P(B|A)+P(\overline{A})P(B|\overline{A})} = \frac{P(A \cap B)}{P(A \cap B)+P(\overline{A} \cap B)} = \frac{P(A \cap B)}{P(B)}$$

## Referencias

- La estadística en Cómic - Larry Gonick y Woollcott Smith