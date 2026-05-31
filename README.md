ЗАДАНИЕ 1
<img width="940" height="490" alt="image" src="https://github.com/user-attachments/assets/c53af842-f1a7-4bdb-a306-fa3384363be9" />

Команды: 
sudo apt update && sudo apt upgrade -y
sudo apt install postgresql postgresql-contrib -y
wget https://repo.zabbix.com/zabbix/7.0/ubuntu/pool/main/z/zabbix-release/zabbix-release_7.0-2+ubuntu24.04_all.deb
sudo dpkg -i zabbix-release_7.0-2+ubuntu24.04_all.deb
sudo apt update
sudo apt install zabbix-server-pgsql zabbix-frontend-php php8.4-pgsql zabbix-apache-conf zabbix-sql-scripts zabbix-agent -y

ЗАДАНИЕ 2

<img width="940" height="358" alt="image" src="https://github.com/user-attachments/assets/2e33c7e7-f7e6-489a-8a55-ef5d862b55a0" />

<img width="940" height="402" alt="image" src="https://github.com/user-attachments/assets/744a3b7e-04a3-4164-8520-a6423a6232a3" />

<img width="623" height="394" alt="image" src="https://github.com/user-attachments/assets/989d43f6-339f-4aa1-ae4f-67abeac91d4b" />

Команды:

sudo apt update
sudo apt install zabbix-agent -y
sudo nano /etc/zabbix/zabbix_agentd.conf
#Server=111.88.155.119
#ServerActive=111.88.155.119
#Hostname=Home-VM (или Cloud-Server) (имя хоста для заббикса)
sudo systemctl restart zabbix-agent
sudo systemctl enable zabbix-agent
sudo systemctl status zabbix-agent
