# oracle-weblogic-12.2.1
Oracle Weblogic Version 12.2.1
#ARCHIVOS REQUERIDOS PARA LA IMAGEN
#(1) fmw_12.2.1.3.0_wls.jar
#Download the Developer Quick installer from http://www.oracle.com/technetwork/middleware/weblogic/downloads/wls-for-dev-1703574.html
(2) jdk-8u161-linux-x64.rpm 
#Download from http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
#Crear directorio de instalador Java
sudo mkdir -p /docker/docker-images-master/OracleJava/java-8
$ pwd
/docker/docker-images-master/OracleJava/java-8
#Mover el instalador Java al directorio requerido
sudo mv ~/Descargas/jdk-8u161-linux-x64.rpm .
#Mover el instalador de weblogic al directorio requerido
sudo mv ~/Descargas/fmw_12.2.1.3.0_wls_Disk1_1of1.zip .
#Descomprimir el zip del instalador
sudo unzip fmw_12.2.1.3.0_wls_Disk1_1of1.zip
#COMO DISENAR LA IMAGEN
Put all downloaded files in the same directory as this Dockerfile
#Run: 
#$ sudo docker build -t oracle/weblogic:12.2.1 . 
