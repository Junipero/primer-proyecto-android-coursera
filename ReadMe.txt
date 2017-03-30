Para los idiomas lo que hice fue crear varios ficheros strings.xml en values, cada uno con su idioma, y dupliqué
el fichero original para mantener las variables. Dupliqué también la variable app_name en caso de que no consiguiese 
quitar la barra de acción puesto que al principio no tenía claro cómo hacerlo.

Para la imagen de fondo, utilicé la función de nine patch que, al contrario que en el video, ya está incluida en la versión actual de
Android Studio, basta con abrir un fichero que acabe en .9.png para que abra el editor. Para generar las 2 zonas de la parte de arriba
hice doble clic en el borde para que generase otra. Después basta con seguir el video del curso para generar un Batch Drawable Import
con el fichero Nine Patch ya editado.

Para el imitar el estilo del botón, generé un drawable llamado button_white_border.xml que dibuja un borde blanco, y lo utilicé como
fondo del botón. Después me limité a poner un textView y anclarlo a la parte superior y a los laterales de la pantalla para asegurarme
de que estuviese siempre centrado aunque cambiase el locale. Además, generé nuevos layouts para landscape, xlarge y xlarge landscape.

Para que los mensajes de bienvenida y del botón cambien automáticamente están referenciados vía @string/mensaje_bienvenida y
@string/mensaje_boton como se indica en el video del curso.

Para eliminar la barra de acción de la parte superior, cambié el theme de la aplicación desde styles.xml, pasando a usar NoActionBar
en lugar de DarkActionBar. 
