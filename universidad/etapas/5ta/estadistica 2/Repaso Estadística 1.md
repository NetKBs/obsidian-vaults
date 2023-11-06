

[[Estadística II]]
/[[Unidad 1 Estadistica Inferencial Y Muestreo  | Siguiente]]
## Indice
- [[#Conceptos Básicos]]
- [[#Distribución De Frecuencias]]
- [[#Medidas De Tendencia Central]]
- [[#Probabilidad (combinatoria)]]
- [[#Medidas De Dispersión]]
- [[#Desviación]]
- [[#Escalas De Medición]]

## Conceptos Básicos
- **Población:** Conjunto de individuos sobre la que se estudia una característica 
<br>
- **Individuo:** también conocido como unidad estadística, es cada uno de los elementos que componen la población
<br>
- **Muestra:** un conjunto representativo de la población
<br>
- **Dato:** cada uno de los valores obtenidos (respuestas)

![[Pasted image 20231025143626.png]]

##### Tipos De Variables

- **Cualitativas:** características o cualidades que no pueden ser medidas con números.
	- *Nominales:* no existe orden
	- *Ordinales:* existe un orden

<br>

- **Cuantitativas:** se expresa mediante un número, se pueden realizar operaciones con ellos.
	- *Discretas:* toman un número finito de valores
	- *Continua:* toma un número infinito de valores


**Ejemplo:**
- Deporte Favorito => Nominal
- Número de pantalones de mis amigos => Discreta
- Medallas ganadas en una competencia => Ordinal
- Peso de compañeros en un salón => Continua


---




## Distribución De Frecuencias

Recomendaciones para elegir si es una tabla de distribución simple o de intervalos: 
- Si hay 12 o menos datos, deberíamos optar por una tabla simple

###### Columnas Generales:

- **f => Frecuencia Absoluta :** el número de veces que se repite un dato
- **F => Frecuencia Absoluta Acumu**lada
- **fr => Frecuencia Relativa:** $f_{ri}=\frac{f_{i}}{n}$
- % => Porcentaje: $\%_{i}=f_{ri}\times100$

### Simple
![[Pasted image 20231028200727.png|400]]

| Días   | f   | F   | fr    | %   |
| ------ | --- | --- | ----- | --- |
| 0      | 6   | 6   | 0.24  | 24  |
| 1      | 7   |     | 0.28  | 28  |
| 2      | 6   | 13  | 0.24  | 24  |
| 3      | 4   | 19  | 0.16  | 16  |
| 4      | 1   | 23  | 0.040 | 4   |
| 5      | 1   | 24  | 0.040 | 4   |
| $\sum$ | 25  | 25  | 1     |     |


### Intervalos

###### Regla De Sturges
Para calcular el número de intervalos 
**(Ambas fórmulas equivalentes)**:
$$K = 1+\log_{2}(n)$$ 
$$K = 1+3,322 \times \log(n)$$ 
*Nota: Siempre se aproxima al número impar más cercano*

###### Pasos Antes De Hacer Una Tabla De Intervalos
- **Paso 1:** Encontrar El Rango $$R = X_{max}-X_{min}$$
- **Paso 2: **Hallar Los Intervalos $$K = 1+3,322 \times \log(n)$$ 
- **Paso 3:** Hallar La Amplitud $$A = {R \over K}$$
  *Nota: Se redondea al número siguiente*

![[Pasted image 20231028202248.png|200]]

Columnas Extras:
**X => Marca De Clase: **es el promedio de cada intervalo $L_{i}+L_{s}\over2$

![[Pasted image 20231028202622.png|400]]

$R= 71-27 =44$
$K = 1+3,322 \times \log(50)=6.65\approx7$
$A = {{44 \over 7}=6,28 \approx7}$

| Velocidad <br> $L_{i}-L_{s}$ | X    | f   | F   | fr    | %   |
| ---------------------------- | ---- | --- | --- | ----- | --- |
| 27-34                        | 30,5 | 3   | 3   | 0,06  | 6   |
| 34-41                        | 37,5 | 1   | 4   | 0,02  | 2   |
| 41-48                        | 44,5 | 4   | 8   | 0,08  | 8   |
| 48-55                        | 51,5 | 28  | 36  | 0,56  | 56  |
| 55-62                        | 58,5 | 12  | 48  | 0,024 | 24  |
| 62-69                        | 65,5 | 1   | 49  | 0,02  | 2   |
| 69-76                        | 72,5 | 1   | 50  | 0,02  | 2   |
| $\sum$                       |      | 50  |     |       | 100 |

---
## Medidas De Tendencia Central
*Datos No Agrupados*

**Media Aritmética (Promedio):** es el valor obtenido al sumar todos los datos y dividir el resultado entre el número total de datos
$$\overline{X}={\sum X_{i} \over N}$$

**Mediana:** el valor que ocupa el lugar central de todos los datos, cuando estos están ***ordenados***. Se representa con $Me$

- **Nro De Datos Impar:** ordenar y seleccionar el valor del centro


- **Nro De Datos Pares:** ordenar y hallar el promedio de los 2 datos centrales


**Moda:** El o los valores que más se repiten. Se representa con  $Mo$. Cuando hay más de dos datos en la moda, se le dice **distribución bimodal**

*Ejemplo: encontrar la media, la moda y la mediana de los siguientes datos:*

**Datos Ordenados:** 40, 41, 42, 45, 45, 46, 47, 47, 48, 49, 50, 53, 54

$$\overline{X}=46.69$$
$$Me = 47$$
$$Mo = 45, 47$$

---

## Probabilidad (combinatoria)

**Experimento Aleatorio: **aquellos experimentos en donde no sabemos el resultado (no se puede predecir el resultado)

**Espacio Muestral (S - Ω) :** el conjunto de todos los resultados posibles de un experimento aleatorio

**Evento o Suceso:** uno o varios de los posibles resultados

*Ejemplo: lanzar 2 monedas al aire*
$$S = \{CC, SS, CS, SC\}$$
*A = La primera sea cara* ***(evento)***
$$A = \{CC,CS\}$$

##### Probabilidad De Un Evento Simple

*Formula De Laplace:* $$P_{(A)}={NumeroDeCasoFavorables\over NumeroDeCasosPosibles}$$

*Ejemplo: se seleccionan tres canicas al azar de una caja que contiene 4 verdes, 2 azules, 1 roja y 3 amarillas. ¿Cuál es la probabilidad de que la tercera canica sea verde? Dado que:*

a) Las dos primeras fueron verdes: ${2\over8}=25\%$ 
b) Las dos primeras fueron amarillas: ${4\over8}=50\%$ 

---

## Medidas De Dispersión

##### Varianza
Promedio de los cuadrados de las desviaciones medidas al rededor de la media. Podemos saber cuánto se alejan los valores individuales respecto al promedio

**Para una población:**
$$\sigma²={\sum(x-\overline{x})² \over n}$$

**Para una muestra:**
$$S²={\sum(x-\overline{x})² \over n-1}$$

##### Desviación Estándar
La raíz cuadrada de la varianza. Podemos saber cuánto se alejan los valores individuales del promedio en términos de la unidad de medida original

$$\sigma = \sqrt{ValorVarianza}$$

---

## Desviación

*Lo representamos con* $D_{x}$

**Respecto A La Media:** es la diferencia en valor absoluto entre cada valor de la variable y la media aritmética.

**Desviación Media:** es el promedio de las desviaciones respecto de la media

---
## Escalas De Medición
Las escalas de medición son los criterios que se usan para asignar valores a las variables, según sus propiedades y características. Las escalas de medición pueden ser de cuatro tipos: nominal, ordinal, de intervalo y de razón

#### Variables Cualitativas
**Nominal:** no tienen un orden natural, como el nombre, el país, el tipo de sangre, etc.  Solo permite clasificar los datos en categorías sin establecer una jerarquía entre ellas. *Ejemplo: el tipo de sangre de una muestra de personas, se puede usar una escala nominal para asignar un valor a cada categoría: A, B, AB, o O*

**Ordinal:** permite ordenar los datos según una jerarquía, pero no indica la distancia o la diferente entre ellos. Por ejemplo, si se estudia a nivel de estudio de una muestra de personas, se puede usar la escala ordinal para asignar un valor a cada categoría: primaria, secundaria, universidad y postgrado
 
#### Variables Cuantitativas
**Razón:** se usa cuando hay un cero absoluto, que significa la ausencia total de lo que se mide. Por ejemplo, si se mide el peso de una persona, se puede usar la escala de razón, porque el cero significa que no hay peso. Se pueden hacer operaciones matemáticas (suma, resta, división y multiplicación), también comparar la proporción y la razón entre valoresx Ejemplo: si una persona pesa 80kg y otra 40kg, se puede decir que la primera pesa el doble que la segunda

**Intervalo:** se usa cuando hay un cero relativo, que no significa la ausencia total de lo que se mide. Por ejemplo, si se mide la temperatura de una persona, se puede usar la escala de intervalo, porque el cero no significa que no hay temperatura. Con esta escala solo se puede sumar y restar. Tampoco se puede comprar la proporción y la razón entre valores

---

[[Unidad 1 Estadistica Inferencial Y Muestreo  | Siguiente]]