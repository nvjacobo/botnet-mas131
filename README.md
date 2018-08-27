
# Botnet contra sitios web de medios independientes en México

Existen grupos que utilizan fallos de la tecnología para hacer negocio, al explotar sus vulnerabilidades con fines específicos; tal fue el caso del ataque informático WannaCry, que secuestra computadoras y dispositivos para posteriormente demandar dinero.

A continuación se da cuenta de la botnet que estuvo detrás del ataque informático al medio de comunicación Másde131 durante 2016, en el contexto de una serie de ataques temporalmente cercanos -y con similitud en técnicas- realizados contra los sitios de Rompeviento TV y Radio Zapote.

La segunda semana de junio de 2016 la infraestructura que hace funcionar el sitio de www.masde131.com detectó que la base de datos encargada de almacenar los contenidos para el sitio había sufrido de una modificación inusual, misma que posteriormente se identificó como realizada por un intruso. Frente a esta situación de inmediato la redacción tomó la decisión de deshabilitar temporalmente el sitio web hasta tener un diagnóstico sobre el nivel de compromiso de la seguridad, con el fin de proteger la navegación de los lectores y editores.

El proceso de análisis inició con la preservación de los registros del sistema y sus configuraciones, para después extraerlos. Dichos registros permiten reconstruir las diferentes fases, técnicas involucradas y su desarrollo para determinar el nivel de compromiso; en otras palabras, los niveles de control que el atacante logró obtener ya sea parcial o completamente.

A través de pruebas de integridad de los archivos antes mencionados, los análisis identificaron lo siguiente:

 1. El atacante logró obtener el control de un usuario con privilegios para escribir artículos, no para publicarlos, esto fue logrado por medio de intentos continuos de acceso con contraseñas aleatorias.
    
 2. Con este acceso intentó repetidamente modificar las últimas entradas para colocar etiquetas html que permitieran introducir anuncios.

Una vez que logró determinarse el nivel de compromiso se decidió ejecutar un plan de recuperación desde los respaldos, tomando consideraciones y medidas de seguridad; entre ellas, un sistema especial de contención contra ataques desarrollado por Deflect de la organización Equalit.ie. Posteriormente, la investigación continuó para conocer más sobre el perfil del ataque y documentar la infraestructura involucrada.

Algunos de los requerimientos para materializar un ataque como el tratado aquí son capacidades de ancho de banda y procesamiento para realizar las peticiones de forma continua, recurrente y automática. Existen varias maneras documentadas sobre cómo obtener máquinas con ancho de banda y procesamiento para realizar los ataques, una de ellas es alquilándolas o pagando por la infraestructura directamente; otra es por medio de control remoto de computadoras o dispositivos de otras personas, usando una parte de sus recursos disponibles para así tener un conjunto de computadoras… Lo que también se conoce como un tipo de botnet.

La botnet que realizó el ataque contra el Másde131 contaba con al menos 25 mil direcciones IP, de las cuales tomamos una muestra de 1200 para posicionarla en un mapa a modo que la dirección geográfica correspondiera con el registro asociado. Esto quiere decir que cada punto en el mapa está asociado a un registro de dichas direcciones, aunque esto no necesariamente implique que la conexión provenga de los puntos señalados.

Un análisis coincidente por técnica e infraestructura, que incluso comparte varias de las direcciones IP con este caso, fue publicado por la empresa WordFence a comienzos de este año. El reporte de WordFence apunta a que una vez que la botnet logra el control de algún sitio web, busca colocar banners de anuncios de Google en los archivos de encabezado del sitio comprometido como una forma de monetizar el ataque.

Explotar la vulnerabilidad de una contraseña débil en el sitio made131.com, permitió que se obtuviera el control temporal sobre su base de datos. Sin embargo lo que realmente permitió realizar el ataque es un problema exponencial en el que estamos involucradas todas las personas que usamos tecnología, así como los fabricantes y proveedores de servicios; ya que nuestra relación con la tecnología genera un espacio en el que pueden existir grupos que exploran modelos de negocio desde la explotación de vulnerabilidades tecnológicas para generar ganancias.







