## Análisis estructural de Twitter como sistema orientado a objetos

Twitter puede descomponerse en varias clases y objetos que interactúan entre sí para proporcionar las funcionalidades descritas anteriormente. A continuación, se describe un análisis preliminar de las clases principales que podrías considerar para un diagrama de clases.

### 1. Clase Usuario (User)

    Atributos:
        nombreUsuario: String
        idUsuario: Integer
        biografia: String
        seguidores: Lista de usuarios
        seguidos: Lista de usuarios
        tweets: Lista de tweets
        mensajesDirectos: Lista de mensajes directos
    Métodos:
        twittear(): Crear un nuevo tweet
        seguirUsuario(Usuario): Seguir a otro usuario
        dejarDeSeguir(Usuario): Dejar de seguir a un usuario
        enviarMensaje(Usuario, Mensaje): Enviar un mensaje directo
        verTimeline(): Mostrar los tweets de las cuentas seguidas

### 2. Clase Tweet

    Atributos:
        idTweet: Integer
        contenido: String
        fecha: DateTime
        autor: Usuario
        retweets: Lista de usuarios que han retuiteado
        likes: Lista de usuarios que han dado "me gusta"
    Métodos:
        retweet(): Retuitear el tweet
        darLike(): Dar "me gusta" al tweet
        responder(Tweet): Responder al tweet
        mostrar(): Mostrar el contenido del tweet

### 3. Clase Mensaje (DM - Direct Message)

    Atributos:
        idMensaje: Integer
        contenido: String
        fechaEnvio: DateTime
        remitente: Usuario
        receptor: Usuario
    Métodos:
        enviar(): Enviar el mensaje
        leer(): Leer el contenido del mensaje

### 4. Clase Hashtag

    Atributos:
        idHashtag: Integer
        texto: String
        tweetsAsociados: Lista de tweets que contienen el hashtag
    Métodos:
        agregarTweet(Tweet): Asociar un tweet al hashtag
        mostrarTweets(): Mostrar todos los tweets que usan el hashtag

### 5. Clase Notificacion

    Atributos:
        idNotificacion: Integer
        tipo: String (mención, retweet, me gusta, etc.)
        remitente: Usuario que genera la acción
        fecha: DateTime
    Métodos:
        mostrarNotificacion(): Mostrar los detalles de la notificación

### 6. Clase Timeline

    Atributos:
        idTimeline: Integer
        usuarioPropietario: Usuario
        tweets: Lista de tweets
    Métodos:
        actualizar(): Actualizar el timeline con nuevos tweets de las cuentas seguidas
        mostrar(): Mostrar los tweets del timeline en tiempo real

- Más información sobre cada clase en el apartado de Detalle_Clases
