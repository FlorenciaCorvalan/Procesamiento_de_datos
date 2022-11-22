# Procesamiento_de_datos

Para la realización del proceso se asumió que el archivo es dejado en una ubicación específica, como por ejemplo FileServer (podría ser un File System).
El gestor de base de datos utilizado es MySQL.

Para reproducir correctamente la notebook de forma local se debe:
-Configurar la direccion donde se encuentra el archivo, que se encuentra en la celda 4:
archivo = ('Documentos/FileServer/ACARA '+str(mes)+'-'+str(anio)+'.csv')

-Configurar la conexión a la base de datos local, que se encuentra en la ultima celda:
conection = mysql.connector.connect(user='root', host='localhost', password='tupassword', database='Acara',  auth_plugin='mysql_native_password')
