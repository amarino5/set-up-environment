#Documentacion de instalacion de entorno Ubuntu
##Instalacion de guest utils de ubuntu para permitir el copy-paste entre anfitrion y maquin virtual

~~~javascript
sudo apt-get install virtualbox-guest-dkms
sudo apt-get install virtualbox-guest-utils virtualbox-guest-x11
~~~

Reiniciar tras la instalación

##Instalacion de git
~~~ javacript apt-get install git ~~~
###configure remote repo
~~~ javascript git config --global user.name YOUR NAME
git config --global user.email YOUR EMAIL ADDRESS
~~~
##Generate ssh-keys
~~~ javascript ssh-keygen -t rsa -b 4096 -C your_email@example.com
~~~
--https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/
##Install and download Anaconda
-https://www.continuum.io/downloads#_unix
./Anaconda2-4.0.0-Linux-x86_64.sh
##Install RStudio and interpreter
-https://www.rstudio.com/products/rstudio/download/
sudo apt-get dpkg
sudo dpkg -i rstudio-0.99.902-amd64.deb 
sudo apt-get install -f
sudo dpkg -i rstudio-0.99.902-amd64.deb 
sudo apt-get -y install r-base
rstudio
##Install python IDE pycharm
--https://www.jetbrains.com/pycharm/
gunzip pycharm-community-2016.1.4.tar.gz 
tar -xvf pycharm-community-2016.1.4.tar
cd pycharm-community-2016.1.4/bin
./pycharm

##Instal MongoDB
https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/
###Start mongo service 
~~~javascript
sudo service mongod start
~~~


mongod --dbpath /mongodb/data/db
##DOnwload Robomongo
--https://robomongo.org/download
~~~javascript mv Downloads/robomongo-0.9.0-rc8-linux-x86_64-c113244.tar.gz /software
~~~javascript cd /software
~~~javascript gunzip robomongo-0.9.0-rc8-linux-x86_64-c113244.tar.gz
~~~javascript tar -xvf robomongo-0.9.0-rc8-linux-x86_64-c113244.tar
~~~
##Download and install protege
--http://protege.stanford.edu/download/protege/4.3/installanywhere/Web_Installers/
