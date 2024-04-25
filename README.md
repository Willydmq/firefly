# firefly
Este archivo Docker Compose crea dos servicios: firefly_iii_app y firefly_iii_db. El servicio firefly_iii_app utiliza la imagen de Firefly III y se conecta a la base de datos que se crea con el servicio firefly_iii_db.

Por favor, asegúrate de cambiar los valores de las variables de entorno (FF_APP_KEY, MYSQL_ROOT_PASSWORD, MYSQL_DATABASE, MYSQL_USER, MYSQL_PASSWORD) por los que desees usar en tu entorno.

Además, este archivo Docker Compose mapea dos volúmenes del contenedor Firefly III a tu sistema de archivos local (./firefly_iii_export y ./firefly_iii_upload), lo que te permite acceder a los datos exportados e importados directamente desde tu máquina local.

he cambiado el puerto de la base de datos a 3307. Recuerda que debes cambiar este valor en dos lugares: en la variable de entorno FF_DB_PORT del servicio firefly_iii_app y en la sección de puertos del servicio firefly_iii_db.
