---

layout: post
title:  "Just fancy words"
date:   2022-01-01 09:30:00 -0300
categories: jekyll update

---

Paso a citar un fragmento de un manual de referencia técnica de un dispositivo que estamos utilizando en un proyecto (traducido al Español):

> Los dispositivos que requieren interacción con la CPU también intercambian datos
> con dicha CPU. Sin embargo, cuando la CPU produce datos (compartidos), dichos datos 
> normalmente son guardados en caché para mejorar el desempeño. Hay dos maneras de compartir
> datos entre dispositivos y CPUs:
> * En coherencia por software, el software (como productor) debe vaciar las cachés de
> las CPUs antes de que los dispositivos puedan leer datos compartidos desde la memoria.
> Y si es el dispositivo el productor de los datos, es el software (como consumidor)
> quien debe invalidar las cachés de las CPUs antes de utilizar los datos producidos
> por el dispositovo.
> * La coherencia por hardware (coherencia de Entrada/Salida) puede proveer coherencia
> de datos al causar que las peticiones de memoria _pispeen_ las cachés de las CPUs.
> Esto aumenta la velocidad de la compartición de datos significativamente (al evitar
> vaciar/invalidar las cachés), y simplifica el software.

A simple vista, a muchos esto podría sonarle _chino básico_. Obviando el hecho de que ni siquiera un experto entiende explicaciones complicadas sin contexto alguno, podemos estar de acuerdo en que este par de párrafos supone que el lector comprende un conjunto bastante extenso de conceptos técnicos específicos. Personalmente, no habría entendido el texto entero de haberlo leído un año atrás; pero 



hay ciertas cosas que sencillamente son muy difíciles de _explicar con peras_. la física cuántica o la matemática muy abstracta se me vienen a la cabeza como cosas que siempre me costaron mucho porque me costaba encontrar en ella analogías con cosas cotidianas. 

pero lo sorprendente de la ingeniería moderna es que gran parte de ella está basada en una enorme acumulación minuciosa y paciente de formalizaciones nacidas de conceptos sencillos más que de grandes ideas muy complejas. 

casi todas las cosas con las que trabajo a diario me hacen imaginar comparaciones con problemáticas similares que cualquiera de nosotros enfrenta en su vida cotidiana: las fábricas, el tránsito y los deportes grupales son campos minados de potenciales ejemplos.

qué sucede con la frase de arriba? es natural no entenderla porque está cargada de jerga, pero hagamos el intento de explicarla en términos sencillos y verán a qué me refiero.

Empecemos por una relación de compromiso fundamental de la electrónica moderna: todo tipo de memoria donde uno quiere guardar información, cuánto más rápida es más cara, más difícil de fabricar y consume más energía. Una computadora o teléfono celular modernos tiene mucho tipo de memorias: poquito de la más rápida, una cantidad mediana de la más o menos ligera, y mucho de la más lenta. 

Un ejemplo universal cuando se habla de arquitectura de computadoras es el siguiente: el procesador es un cocinero, toma ingredientes y les da un valor agregado a través de cierto proceso. Cuándo el cocinero planea una gran cena, se asegura de tener todos los ingredientes en su heladera o alacena con anterioridad. Va al mercado, y compra todo lo necesario. Cuando llega la hora de cocinar, busca todo lo necesario en la heladera y lo pone a mano, en su mesada. En esta analogía, el mercado es el equivalente a un dispositivo de almacenamiento masivo, como un disco duro o tarjeta de memoria. La heladera/alacena, es la famosa memoria RAM. Y la mesada, las mencionadas anteriormente memorias _caché_. Han visto cuando un videojuego o programa carga una famosa barrita de progreso? Usualmente eso significa que la información necesaria se está llevando de disco a memoria.

 Como se habrán imaginado, leer y escribir a disco es muy lento, así como ir a comprar ingredientes adicionales cuando ya estamos cocinando. Y nuestra mesada es muy pequeña, así que a veces no entra todo lo que necesitamos, pero es mucho más rápido ir a la heladera que al mercadito. 

Con esta limitación en mente se han desarrollado 50 años de sistemas y programas. Listo, sigamos a otra cosa.

Qué pasa cuando la memoria más rápida es más chica que la más lenta? Lo adivinaron, hay que repetidamente usarla para distintas cosas. 


