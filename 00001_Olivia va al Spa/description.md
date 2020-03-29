Queremos estudiar el efecto que produce visitar un spa.

Cuando el `spa` atiende una persona pasan dos cosas: la persona recibe masajes, y se da un baño de vapor.

Inicialmente vamos a querer que Olivia pueda atenderse en el spa. Sabemos que:

* cuando Olivia **recibe masajes**, su grado de concentración aumenta 2 puntos, pero a partir del tercer masaje, al estar más relajada su grado de concentración aumenta 5 puntos.
* cuando **se da un baño de vapor**, su grado de concentración aumenta 1 punto.
* si Olivia tiene 7 puntos o más de concentración, **es feliz**.
* cuando **discute**, su grado de concentración baja a 5, salvo que tenga menos de 5 puntos de concentración, en cuyo caso no pasa nada.

Además necesitamos poder consultar su grado de concentración. El valor inicial para la concentración de Olivia es 4, pero debe poder cambiar dependiendo de lo que haga como se indicó anteriormente.

Definir los objetos `spa` y `olivia` de modo que se puedan usar de esta forma:

```wollok
ム olivia.discutir()
ム olivia.gradoDeConcentracion()
ム olivia.esFeliz()
ム olivia.recibirMasajes()
ム olivia.darseUnBanioDeVapor()
ム spa.atender(olivia)
```

> Los objetos `olivia` y `spa` pueden entender otros mensajes además de los mencionados, pero no se imponen restricciones sobre los mismos.