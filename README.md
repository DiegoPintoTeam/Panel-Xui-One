apt-get update

apt-get upgrade

wget "https://update.xui.one/XUI_1.5.12.zip" -O /tmp/XUI_1.5.12.zip

cd /tmp

apt install zip unzip -y ; unzip XUI_1.5.12.zip

./install

wget "https://github.com/DiegoPintoTeam/Panel-Xui-One/raw/main/xui_crack.tar.gz" -O /tmp/xui_crack.tar.gz

cd /tmp

tar -xf xui_crack.tar.gz

sh /tmp/install.sh

---------------------------------------------------------------------
Restaurar Base de datos

/home/xui/tools migration "/root/backup.sql" 

/home/xui/bin/php/bin/php /home/xui/includes/cli/migrate.php
