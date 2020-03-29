Queremos hacer nuestra propia red social en la cual el contenido publicado por los usuarios pueda ser visible por otros usuarios de la red, dependiendo de cómo se haya creado dicho contenido.

Cuando se crea una publicación se registra el usuario que creó la publicación y la fecha de publicación. La misma puede ser pública (puede verla cualquier usuario de la red) o privada, haciendo que sea visible sólo por los contactos de quien hizo la publicación.

Además algunas publicaciones, a las que denominamos historias, sólo son visibles hasta el día siguiente de su publicación por aquellos usuarios que correspondan de acuerdo a si era pública o no. Independientemente de todo esto, quien realiza la publicación **siempre puede ver su propio contenido publicado**.

- Debe ser posible en cualquier momento hacer que una publicación o historia se vuelva pública o privada. Para ello se espera que las publicaciones e historias entiendan los mensajes `volverPrivada` y `volverPublica`.
- Se tiene que poder consultar si una publicación o historia puede verla un determinado usuario en una fecha.

Ejemplo de uso:

```Wollok
ム var otroDia = historiaPublica.fechaPublicacion().plusDays(1)
ム historiaPublica.puedeVerla(new Usuario(), otroDia)
  => true
ム historiaPublica.volverPrivada()
ム historiaPublica.puedeVerla(new Usuario(), otroDia)
  => false

ム var usuarioQueCreoLaPublicacion = publicacionPrivada.creador()
ム publicacionPrivada.puedeVerla(usuarioQueCreoLaPublicacion, new Date())
  => true
```

> Además de definir las clases y/u objetos necesarios para resolver el problema, declarar las constantes  `historiaPublica` y `publicacionPrivada` para usarlas desde las pruebas, instanciando los objetos necesarios para poder usarlos como en el ejemplo.

> La clase Usuario ya está definida, podés verla en la biblioteca.