## 6. Clase Timeline

### El Timeline es la vista principal donde el usuario ve los tweets de las cuentas que sigue.

    Atributos:

        idTimeline: Integer
        usuarioPropietario: Usuario
        tweets: Lista de tweets


    Métodos:

        actualizar(): Actualizar el timeline con nuevos tweets de las cuentas seguidas
        mostrar(): Mostrar los tweets del timeline en tiempo real


    Atributos adicionales:

        tweetsDestacados: Lista de tweets (tweets recomendados o promocionados).


    Métodos adicionales:

        filtrarPorHashtag(Hashtag): Filtra el timeline por tweets que contienen un hashtag específico.
        ordenarPorReciente(): Ordena los tweets por fecha de publicación.
        agregarTweet(): Añade un tweet al timeline.
        marcarComoVisto(Tweet): Marca un tweet en el timeline como visto.


Relaciones:

    Un timeline contiene muchos tweets (relación uno a muchos con Tweet).
