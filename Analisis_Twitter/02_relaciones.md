Relaciones entre clases

    Usuario y Tweet:

        Tipo de relación: Composición.
        Justificación: Un Usuario "posee" sus Tweets, es decir, si un usuario es eliminado, sus tweets también se eliminan. Los tweets no pueden existir sin un usuario que los haya creado.


    Usuario y Mensaje (Direct Message):

        Tipo de relación: Agregación.
        Justificación: Los Mensajes pueden existir independientemente de los usuarios, ya que un mensaje es un intercambio temporal. Sin embargo, los mensajes se asocian a usuarios como remitente y receptor.


    Tweet y Hashtag:

        Tipo de relación: Dependencia.
        Justificación: Un Tweet puede tener uno o varios Hashtags, pero un Hashtag no depende de un tweet específico para existir. Los tweets utilizan hashtags temporalmente para organizarse.


    Tweet y Notificacion:

        Tipo de relación: Dependencia.
        Justificación: Un Tweet puede generar una Notificación, pero las notificaciones solo son "invocadas" cuando ocurre una acción (retweet, mención, etc.). No existe una dependencia permanente entre ellos.


    Timeline y Tweet:

        Tipo de relación: Agregación.
        Justificación: Un Timeline contiene múltiples Tweets, pero estos tweets no dependen del timeline para existir. Los tweets simplemente se agregan temporalmente al timeline de un usuario.


    Usuario y Timeline:

        Tipo de relación: Composición.
        Justificación: Cada Usuario tiene un único Timeline, el cual está directamente asociado al usuario. Si un usuario se elimina, también se elimina su timeline.
