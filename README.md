#Documentacion de instalacion de entorno Ubuntu
##Instalacion de guest utils de ubuntu para permitir el copy-paste entre anfitrion y maquin virtual

~~~javascript
sudo apt-get install virtualbox-guest-dkms
sudo apt-get install virtualbox-guest-utils virtualbox-guest-x11
~~~

Reiniciar tras la instalación

##Instalacion de git
~~~ javacript 
apt-get install git 
~~~

###configure remote repo
~~~ javascript 
git config --global user.name YOUR NAME
git config --global user.email YOUR EMAIL ADDRESS
~~~

##Generate ssh-keys
~~~ javascript 
ssh-keygen -t rsa -b 4096 -C your_email@example.com
~~~
--https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/

##Install and download Anaconda
-https://www.continuum.io/downloads#_unix

./Anaconda2-4.0.0-Linux-x86_64.sh

##Install RStudio and interpreter
-https://www.rstudio.com/products/rstudio/download/
~~~javascript
sudo apt-get dpkg
sudo dpkg -i rstudio-0.99.902-amd64.deb 
sudo apt-get install -f
sudo dpkg -i rstudio-0.99.902-amd64.deb 
sudo apt-get -y install r-base
~~~

###Ejecutar como:
rstudio

##Install python IDE pycharm
--https://www.jetbrains.com/pycharm/
~~~javascript
gunzip pycharm-community-2016.1.4.tar.gz 
tar -xvf pycharm-community-2016.1.4.tar
cd pycharm-community-2016.1.4/bin
./pycharm
~~~

##Instal MongoDB
https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/

###Start mongo service 
~~~javascript
sudo service mongod start
~~~
###O bien ejecutar indicando el path donde almacena la informacion
~~~javascript
mongod --dbpath mongodb/data/db/
~~~
##Donwload Robomongo
--https://robomongo.org/download
~~~javascript 
mv Downloads/robomongo-0.9.0-rc8-linux-x86_64-c113244.tar.gz /software
cd /software
gunzip robomongo-0.9.0-rc8-linux-x86_64-c113244.tar.gz
tar -xvf robomongo-0.9.0-rc8-linux-x86_64-c113244.tar
cd robomongo-0.9.0-rc8-linux-x86_64-c113244/bin
./robomongo
~~~

##Install Chrome
~~~javascript
wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add - 
sudo sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'
sudo apt-get update 
sudo apt-get install google-chrome-stable
~~~

#Download and install protege
--http://protege.stanford.edu/download/protege/4.3/installanywhere/Web_Installers/

Ejecutar las siguientes lineas antes de ejecutar el paquete descargado.
~~~javascript
 sudo apt-get install libc6-i386 
~~~
##Installing Oracle Java 8
--http://www.webupd8.org/2012/09/install-oracle-java-8-in-ubuntu-via-ppa.html
~~~javascript 
sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer
~~~
##Una vez descargado el protege, ejecutar la instalacion del binario
~~~javascript 
install_protege_4.3.bin
~~~
###Todavia no he conseguido que funcione el ejecutable...en depuracion...

#Install R kernel into Jupyter HUB
~~~ javascript 
conda install -c r r-essentials 
~~~
