# Probabilidad Bayesiana

El Teorema de Bayes es una fórmula que describe cómo actualizar nuestras creencias sobre una hipótesis en función de la evidencia. Se utiliza en una amplia variedad de contextos, incluyendo la detección de spam en los correos electrónicos.

## Teorema de Bayes

El Teorema de Bayes se puede expresar de la siguiente manera:

$$ P(A|B) = \frac{P(B|A) \times P(A)}{P(B)} $$

donde:

- $P(A)$ y $P(B)$ son las probabilidades *a priori* de dichos eventos. Las probabilidades de que dichos eventos sucedan sin estar condicionados por ningún otro evento.
- $P(A|B)$ es la probabilidad condicional o *a posteriori* de la hipótesis $A$ dado el evento $B$, o sea: la probabilidad de que A se dé dado que B se ha dado.

## Ejemplo del teorema de Bayes aplicado a un filtro de *spam*

Supongamos que estamos construyendo un filtro de spam y queremos determinar la probabilidad de que un correo electrónico sea spam, $P(S)$, dado que contiene una palabra específica, $X$, por ejemplo, "oferta". Usando el Teorema de Bayes, podemos expresar esto como:

$$ P(S|X) = \frac{P(X|S) \times P(S)}{P(X)} $$

donde:

- $P(S|X)$ es la probabilidad de que un correo electrónico sea spam dado que contiene la palabra "oferta".
- $P(X|S)$ es la probabilidad de que un correo electrónico, siendo spam, contenga la palabra "oferta".
- $P(S)$ es la probabilidad *a priori* de que cualquier correo electrónico sea spam.
- $P(X)$ es la probabilidad total de que cualquier correo electrónico contenga la palabra "oferta".

Al calcular estas probabilidades y sustituirlas en la fórmula del Teorema de Bayes, podemos obtener una probabilidad actualizada de que un correo electrónico sea spam dado que contiene la palabra "oferta".

Esta versión simplificada al mínimo, puede extenderse a múltiples palabras y características para mejorar la precisión del filtro de spam, y puede irse actualizando (y por tanto, afinando) a medida que se reciben nuevos emails.

## Material complementario

- [3Blue1Brown - Bayes theorem, the geometry of changing beliefs](https://www.youtube.com/watch?v=HZGCoVF3YvM)  
- [Veritasium - The Bayesian Trap](https://www.youtube.com/watch?v=R13BD8qKeTg) ([Versión doblada al español](https://www.youtube.com/watch?v=D7KKlC0LOyw))
- [3Blue1Brown - The medical test paradox, and redesigning Bayes' rule](https://www.youtube.com/watch?v=lG4VkPoG3ko)
- https://www.upgrad.com/blog/bayes-theorem-explained-with-example-complete-guide/
- https://courses.cs.washington.edu/courses/cse312/18wi/312A/lecture7.pdf
