# TC2008B: Evidencia 1

## Game of live: Codiv-19 en Python

_Para usar el código que se presenta se necesita tener instalado mesa.
Con el siguiente comando desde la terminal se puede instalar mesa:_

```
$ pip install mesa
```

### Descripción
El juego de la vida (Game of Live) está basado en los estados que podemos darle a un agente según las reglas que nosotros decidamos que son mejores para la simulación, en este caso en específico las reglas son:
- Si hay menos de dos vecinos contagiados, se está saludable.
- Si hay más de un vecino contagiado, se contagia.
- Cuando un agente está contagiado y tiene más de dos vecinos contagiados se muere.
- Si un agente está contagiado y no tiene vecinos contagiados, vuelve a estar saludable.

Lo que nos hace tener tres estados para cada agente:
- Saludable.
- Contagiado.
- Muerto.

### Variables y parámetros:

Dentro de la simulación tenemos diversas maneras de trabajar con las reglas, puesto que se pueden modificar según queramos hacer las pruebas. Donde empezamos con un número de agentes saludables, y decidir los parámetros de contagio, recuperación o mortalidad.

Para esta simulación en concreto tenemos que cuando un agente saludable esté cerca de al menos un agente contagiado, el primero pasa a estar contagiado. De manera similar, cuando un agente contagiado tiene menos de dos vecinos contagiados, vuelve a estar saludable y para que un agente muera tiene que tener al menos dos vecinos contagiados.

### Resultados:

Las gráficas que se nos dan al final de la simulación tenemos cuántos agentes se contagiaron y cuantos se recuperaron.
Dentro del apartado visual de la simulación podemos ver cómo es que se contagian, recuperan o mueren con el paso del tiempo.
Una de las desventajas de esta simulación es que no logré encontrar una manera de hacer que los agentes con estado de muerto se mantuvieran de esa forma, por ende pueden volver a la vida o contagiarse nuevamente.
De igual manera algunos agentes se quedan con el estado contagiado puesto que están rodeados de agentes muertos, lo que podría hacer que se curaran al no estar cerca de otros agentes contagiados.



