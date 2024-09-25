## 4. Clase Hashtag

### Los hashtags permiten agrupar conversaciones bajo un mismo tema.

    Atributos:

        idHashtag: Integer
        texto: String
        tweetsAsociados: Lista de tweets que contienen el hashtag


    Métodos:

        agregarTweet(Tweet): Asociar un tweet al hashtag
        mostrarTweets(): Mostrar todos los tweets que usan el hashtag


    Atributos adicionales:

        trending: Boolean (indica si el hashtag es tendencia).
        popularidad: Integer (número de veces que se ha usado el hashtag).


    Métodos adicionales:

        buscarTweets(): Busca todos los tweets que contienen el hashtag.
        marcarComoTrending(): Establece el estado de tendencia para el hashtag.


Relaciones:

    Un hashtag puede estar en muchos tweets y un tweet puede tener muchos hashtags (relación muchos a muchos con Tweet).
