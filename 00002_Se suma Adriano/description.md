Continuando con el problema anterior, queremos agregar un nuevo cliente para nuestro spa.

Adriano es programador y nos interesa saber qué tan contracturado está (0 es "nada contracturado", cuanto más alto sea ese número, más contracturado está), y si está fresco para programar. Inicialmente tiene 5 de nivel de contractura y está fresco para programar.

Las acciones relevantes que tiene para este modelo son:

* cuando recibe masajes, baja dos puntos su nivel de contractura. OJO nunca puede ser negativo, o sea, si estaba en 1 pasa a 0, si estaba en 0 se queda en 0.
* cuando se da un baño de vapor, queda fresco para programar.
* al comerse un Big Mac queda fresco para programar (?, así lo definió el usuario).
* cuando codea, su nivel de contractura aumenta 1 punto si está fresco, y en caso contrario aumenta 3 puntos. Indefectiblemente queda quemado para programar (lo opuesto a fresco) cada vez que codea.
* un dia de trabajo de Adriano consiste en: codear, comerse un Big Mac y volver a codear.

Necesitamos que sea posible hacer (por lo menos) lo siguiente:

```wollok
ム adriano.trabajarUnDia()
ム spa.atender(adriano)
ム adriano.nivelDeContractura()
ム adriano.frescoParaProgramar()
```

> Te dejamos tu implementación para el ejercicio anterior en el editor, por si necesitás hacer algún cambio a tu solución además de agregar al objeto `adriano` con el comportamiento indicado.

> Tené en cuenta que la funcionalidad del ejercicio anterior debe seguir andando.