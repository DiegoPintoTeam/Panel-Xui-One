Instalación de panel XUI One

Versión oficial 1.5.5

```
apt-get update; apt-get upgrade; wget "https://update.xui.one/XUI_1.5.5.zip" -O /tmp/XUI_1.5.5.zip; cd /tmp; apt install zip unzip -y ; unzip XUI_1.5.5.zip; ./install; wget "https://github.com/DiegoPintoTeam/Panel-Xui-One/raw/main/xui_crack.tar.gz" -O /tmp/xui_crack.tar.gz; cd /tmp; tar -xf xui_crack.tar.gz; sh /tmp/install.sh
```

Versión beta 1.5.12

```
```
apt-get update
```
```
apt-get upgrade
```
```
wget «https://update.xui.one/XUI_1.5.12.zip» -O /tmp/XUI_1.5.12.zip
```
```
cd /tmp
```
```
apt install zip unzip -y ; unzip XUI_1.5.12.zip
```
```
./install
```
```
wget "https://github.com/DiegoPintoTeam/Panel-Xui-One/raw/main/xui_crack.tar.gz" -O /tmp/xui_crack.tar.gz
```
```
cd /tmp
```
```
tar -xf xui_crack.tar.gz
```
```
sh /tmp/install.sh


Les dejo algunos comandos en caso de fallas:




Iniciar XUI: Utilice el comando
```
/home/xui/service start
```
Detener XUI: Utilice el comando 
```
/home/xui/service stop
```
Ver estado de la base de datos : Utilice el comando 
```
/home/xui/status
```
Herramientas de listado: Utilice el comando
```
/home/xui/tools
```
Crear rescatar Código de Acceso: Utilice el comando
```
/home/xui/tools rescue
```
Crear rescatar Admin Usuario: Utilice el comando
```
/home/xui/tools user
```
Reautorización de equilibradores de carga En MySQL: Utilice el comando
```
/home/xui/tools mysql
```
Restaurar una base de datos en blanco: Utilice el comando
```
/home/xui/tools database
```
Borrar la base de datos de migración: Utilice el comando
```
/home/xui/tools migration
```
Flushing Todos los IPs bloqueados: Utilice el comando
```
/home/xui/tools flush
```
Restauración de puertos de MySQL: Utilice el comando 
```
/home/xui/tools ports
```
Restauración del Código de Acceso de MySQL: Utilice el comando 
```
/home/xui/tools access
```
Generar rápidamente Copia de seguridad completa: Utilice el 
comando 
```
mysqldump -u root xui > xuiLT-backup.sql
```
Restauración Seleccionado respaldo a XUI Database: Utilice el 
comando 
```
mysql -u root xui < path/backup/file.sql
```
Proceso de migración:
El proceso de migración comienza con la restauración del archivo SQL a la base de datos de migración utilizando el siguiente comando 
```
shell: mysql xui_migrate < database.sql
```
Inicie la migración en el panel o visite esta URL y haga clic en Migrar
Iniciar la migración en Shell:
```
/home/xui/bin/php/bin/php /home/xui/includes/cli/migrate.php
```
Iniciar la migración en el navegador:
Visite: http://host.com:port/accesscode/setup

Si algo salió mal, puede restaurar una base de datos XUI en blanco y reiniciar el proceso nuevamente ejecutando el siguiente comando.
```
mysql xui < /home/xui/bin/install/database.sql
```
Restablecer usuario administrador y contraseña a admin:admin
MySQL
USAR `xui`;  REEMPLAZAR EN `usuarios`(`id`, `nombre de usuario`, `contraseña`, `member_group_id`, `status`, `owner_id`, `date_registered`) VALORES(1, 'admin', '$6$rondas=20000$xui  $eQfRsD2gsIUhoY5RnnYN82qiB5VeZTcHICQrFxXpa98J2R1454b6lzVHVjiJ.NP0gi0X3K7NXVgxeR1VhVhg61', 1, 1, 0, UNIX_TIMESTAMP());
 
Reparar error de licencia
```
/home/xui/status
```
Api Key IMDB
```
3ec71207d069c9fbbb5ef345fa097c72
```

