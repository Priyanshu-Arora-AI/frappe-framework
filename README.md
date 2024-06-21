# frappe-framework



sudo apt-get update -y
sudo apt-get upgrade -y

sudo apt-get install git
sudo apt-get install python3-dev python3.10-dev python3-setuptools python3-pip python3-distutils
sudo apt-get install python3.10-venv
sudo apt-get install software-properties-common
sudo apt install mariadb-server mariadb-client
sudo nano /etc/mysql/my.cnf
Add the following block of code exactly as is:

[mysqld]
character-set-client-handshake = FALSE
character-set-server = utf8mb4
collation-server = utf8mb4_unicode_ci

[mysql]
default-character-set = utf8mb4

sudo apt-get install redis-server
sudo apt-get install xvfb libfontconfig wkhtmltopdf
sudo apt-get install libmysqlclient-dev

sudo mysql_secure_installation
sudo apt install curl


source ~/.profile


curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
nvm install 20
node -v # should print `v20.14.0`

# verifies the right NPM version is in the environment
npm -v # should print `10.7.0`

sudo apt-get install npm
sudo npm install -g yarn
sudo pip3 install frappe-bench
bench init --frappe-branch version-15 frappe-bench

cd frappe-bench
chmod -R o+rx /home/$USERNAME


bench new-site [site-name]
bench get-app payments

bench get-app --branch version-15 erpnext
bench start
