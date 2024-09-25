## 5. Clase Notificacion

### Las notificaciones informan al usuario sobre la interacción con sus tweets o su cuenta.

    Atributos:

        idNotificacion: Integer
        tipo: String (mención, retweet, me gusta, etc.)
        remitente: Usuario que genera la acción
        fecha: DateTime


    Métodos:

        mostrarNotificacion(): Mostrar los detalles de la notificación


    Atributos adicionales:

        leida: Boolean (indica si la notificación ha sido vista).
        mensaje: String (mensaje detallando la notificación, como "X te ha seguido").


    Métodos adicionales:

        marcarComoLeida(): Marca la notificación como leída.
        eliminarNotificacion(): Elimina la notificación.


Relaciones:

    Una notificación está asociada a una acción de un usuario sobre otro usuario o sus tweets (relación muchos a uno con Usuario y Tweet).
