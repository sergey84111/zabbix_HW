# Домашнее задание к занятию "`Система мониторинга Zabbix`" - `Topolev-Soldunov Sergey`


### Инструкция по выполнению домашнего задания

---

### Задание 1
https://github.com/sergey84111/zabbix_HW/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-04-10%20165906.png

sudo apt install postgresql

wget https://repo.zabbix.com/zabbix/6.0/debian/pool/main/z/zabbix-release/zabbix-
release_6.0-4%2Bdebian11_all.deb 
dpkg -i zabbix-release_6.0-4+debian11_all.deb 
apt update

sudo apt install zabbix-server-pgsql zabbix-frontend-php php7.4-pgsql zabbix-apache-conf zabbix-sql-
scripts nano -y # zabbix-agent

sudo -u postgres createuser --pwprompt zabbix
sudo -u postgres createdb -O zabbix zabbix

sudo apt install zabbix-agent -y
sudo systemctl restart zabbix-agent
sudo systemctl enable zabbix-agent

nano /etc/zabbix/zabbix_agentd.conf
sudo systemctl restart zabbix-agent.service

---

### Задание 2
https://github.com/sergey84111/zabbix_HW/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-04-10%20170028.png

https://github.com/sergey84111/zabbix_HW/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-04-10%20170515.png

https://github.com/sergey84111/zabbix_HW/blob/main/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-04-10%20170626.png

git add .
git commit
git push https://github.com/sergey84111/zabbix_HW.git





