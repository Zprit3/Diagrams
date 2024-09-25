## 3. Clase Mensaje (DM - Direct Message)

### Los mensajes directos permiten la comunicación privada entre usuarios.

    Atributos:

        idMensaje: Integer
        contenido: String
        fechaEnvio: DateTime
        remitente: Usuario
        receptor: Usuario


    Métodos:

        enviar(): Enviar el mensaje
        leer(): Leer el contenido del mensaje


    Atributos adicionales:

        visto: Boolean (indica si el receptor ha leído el mensaje).
        mensajeOriginal: Mensaje (para identificar si es una respuesta a un mensaje anterior).


    Métodos adicionales:

        eliminarParaTodos(): Elimina el mensaje para ambos usuarios.
        responderMensaje(Mensaje): Responder a un mensaje directo.
        marcarComoLeido(): Marca el mensaje como leído.

Relaciones:

    Un mensaje tiene un remitente y un receptor (relación muchos a uno con Usuario).
