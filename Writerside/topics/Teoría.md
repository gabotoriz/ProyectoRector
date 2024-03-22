# Teoría

## Ecuaciones Diferenciales

Una ecuación diferencial es una ecuación que involucralas derivadasde una función ***desconocida*** (o variable
independiente) con respecto a una o mas varibles (variables independientes).

### Clasificación de las Ecuaciones Diferenciales

Las ecuaciones diferenciales se pueden clasificar de acuerdo a lo siguiente

| **Ecuación Diferencial Ordinaria** | Si la función desconocida depende de ***una sola variable***   |
|------------------------------------|----------------------------------------------------------------|
| **Ecuación Diferencial Parcial**   | Si la función desconocida depende de ***mas de una variable*** |

<!-- ANEXEMOS EJEMPLOS-->

### Orden de una Ecuacion Diferencial

El orden de una ecuación diferencial es el ***indicado por el índice*** que aparece en la derivada mas alta

<!-- ANEXEMOS EJEMPLOS-->

### Grado de una Ecuacion Diferencial

El grado de una ecuación diferencial (que puede escribirse como un polinomio con respecto de las derivadas), es la
potencia que aparece en la derivada mas alta de la ecuación.

### Linealidad

1. La variable dependiente **y** y todas sus derivadas son de primer grado, **i.e.,** la potencia de todo termino en
   donde aparece ***"Y"*** es **uno**
2. La función g(x) es una función dada de la variable ***x***
3. Las funciones de “y” o de las derivadas de “y” tales como
   ```tex
   \begin{equation}
   sen(x), cos(y'''), e^y
   \end{equation}
   ```
   etc, no pueden aparecer en una ecuación diferencial lineal.
   Cuando la ecuación diferencial no es lineal, se dice que es no lineal.

### Solución de una ecuacion diferencial

Una solución a una ecuación diferencial es cualquier ***función*** o ***relación*** que satisface la ecuación dicho en
otras palabras, la reduce a una identidad.

## Ecuaciones Diferenciales Separables

1. Supongamos que una ecuación diferencial de primer orden de la forma
   <code-block lang="tex">
       \begin{equation}
       \frac{dx}{dy} = F(x,y)
       \end{equation}
   </code-block>
2. Un tipo especialmente simple de una ecuación que ocurre a menudo en la práctica es cunado (1) puede ser escrita de la
   siquiente forma
   <code-block lang="tex">
      \begin{equation}
      f(x) dx + g(y) dy = 0
      \end{equation}
   </code-block>
3. Donde un termino se involucra solo a ***x***, mientras que en el otro solo a ***y***. Esta ecuación puede ser
   resuelta inmediatamente por integración. Así la solución general de (2) es
   <code-block lang="tex">
      \begin{equation}
      \int f(x) dx + \int g(y) dy = C
      \end{equation}
   </code-block>
4. Donde C es la constante de integración. Nosotros podemos regresar a la ecuación (2), tomando la diferenica de ambos miembros de (3), y así eliminar C, esto es
    <code-block lang="tex">
      \begin{equation}
      d \int f(x) dx + d \int g(y) dy = dC
      \end{equation}
   </code-block>


- Multipliacion
- Division
- Factorizacion

## Test

- Ejemplos Genearles (Proceso paso a paso)

