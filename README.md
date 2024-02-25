Instalación de panel XUI One


```
apt-get update; apt-get upgrade; wget "https://update.xui.one/XUI_1.5.12.zip" -O /tmp/XUI_1.5.12.zip; cd /tmp; apt install zip unzip -y ; unzip XUI_1.5.12.zip; /install; wget "https://github.com/DiegoPintoTeam/Panel-Xui-One/raw/main/xui_crack.tar.gz" -O /tmp/xui_crack.tar.gz; cd /tmp; tar -xf xui_crack.tar.gz; sh /tmp/install.sh
```


Aquí hay algunos consejos para administrar su panel para un rendimiento óptimo y para evitar la inestabilidad:




Detener XUI One: Utilice el comando 

```
/home/xui/service stop
```

Iniciar XUI One: Utilice el comando

```
/home/xui/service start
```

Ver estado la base de datos : Utilice el comando 

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

Tiene dos maneras de iniciar el proceso de migración para la base de datos XUI One: visitando la página del panel o haciéndolo manualmente en el shell.

Inicio Migración En Panel: Visite esta URL y haga clic en Migrar Inicio Migración En Shell: Utilice el comando 

```
/home/xui/bin/php/bin/php /home/xui/includes/cli/migrate.php
```

