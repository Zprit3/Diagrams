## 1. Clase Usuario (User)

### El Usuario es una clase central en Twitter, ya que toda la actividad gira alrededor de los usuarios.

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


    Atributos adicionales:

        nombre: String (nombre real del usuario)
        fechaCreacionCuenta: DateTime (fecha en la que el usuario creó la cuenta)
        fotoPerfil: String (enlace a la imagen de perfil)
        numeroTweets: Integer (contador de tweets publicados)
        numeroSeguidores: Integer (contador de seguidores)
        numeroSeguidos: Integer (contador de usuarios seguidos)
        configuracionPrivacidad: Boolean (si el perfil es privado o público)


    Métodos adicionales:

        editarPerfil(nombre, biografia, fotoPerfil): Modifica el perfil del usuario.
        bloquearUsuario(Usuario): Bloquear a otro usuario.
        silenciarUsuario(Usuario): Silenciar las publicaciones de otro usuario sin dejar de seguirlo.
        denunciarTweet(Tweet): Reportar un tweet que infringe las normas.

Relaciones:

    Un usuario tiene muchos seguidores y sigue a muchos usuarios (relación de muchos a muchos con la misma clase Usuario).
    Un usuario puede twittear, retuitear y dar "me gusta" a tweets (relación uno a muchos con Tweet).
    Un usuario puede enviar y recibir mensajes directos (relación uno a muchos con Mensaje).
    Un usuario puede tener múltiples notificaciones (relación uno a muchos con Notificacion).
