### Pràctica 1: Instal•lació d'un SGBD 
 
### Part I - INSTAL•LACIÓ SGBD MySQL Percona (màx. 6 punts) 
 
### ENUNCIAT  
 
### Partint d'una màquina CentOS 7 minimal proporcionada pel professor realitza la instal•lació d'un SGBD Percona Server mitjançant el gestor de paquets YUM. 
 
### ENLLAÇOS 
 
### Percona Server 8.0 Doc  
 ### https://www.percona.com/doc/percona-server/8.0/index.html 	 
 
### Instal•lació Percona Server8.0 via YUM Repository   	https://www.percona.com/doc/percona-server/8.0/installation/yum_repo.html 
 
### Instal•lació MySQL via YUM Repository  	https://www.tecmint.com/install-latest-mysql-on-rhel-centos-and-fedora/ 
 
### LLIURAMENT 
 
### El lliurament d'aquesta activitat correspon a la documentació de tots els passos corresponents a la instal•lació per tenir un SGBD MySQL Percona en funcionament. 
### En la documentació cal incloure les captures d'imatges que es cregui convenients així com la webgrafia utilitzada. 
 
### Altres opcions de lliurament: 
### •	Utilitzar aquest document com a plantilla pel lliurament de l’activitat i penjar-la en tasca destinada a aquesta activitat dins del curs Moodle  
### •	Realitzar la documentació sobre un repositori GIT (Bitbucket o GitLab). Utilitzant el format de fitxer MarkDown (MD). (1 punt) 
### •	Dins d'una Wiki. (1 punt) 
 
### Per les dues últimes opcions d'entrega caldrà indicar en el document penjat en el Moodle la URL a on es troba la documentació i afegir el compte del professor com a membre de l'equip de treball. 
 
### REALITZA LA DOCUMENTACIÓ NECESSÀRIA PER LA INSTAL•LACIÓ PAS A PAS. 
 
### •	Indica clarament els passos per reproduir la instal•lació en un altra màquina. 
 
### •	Si realitzes algun canvi en la configuració del firewall, o altres elements de seguretat per poder tenir accés indica quins canvis has hagut de fer. 
 
### •	Cal tenir en compte que la documentació va dirigida a tècnics informàtics i no a usuaris no experts. 
 
### •	Es valorarà la presentació, l'organització del text i la facilitat de lectura. 


### Per instal•lar el SGBD he instal•lat el centos 7 i ens demanarà una contrasenya per l’ usuari root:
![image](https://user-images.githubusercontent.com/99834779/154843717-8fa11e55-9a2c-4b49-afc6-9352def2c15f.png)
### Després quant estigui instal•lat el centos 7 configurem les targetes de xarxa:
### Primer configurem els dos fitxers de xarxa, per entrar al fitxer de xarxaa enp0s3:
![image](https://user-images.githubusercontent.com/99834779/154843709-092cdded-dc6e-4148-89d9-01738f02126f.png)
### Dintre ha d’ estar així, per modifcar les coses de dintre és donant a la tecla “i”:
![image](https://user-images.githubusercontent.com/99834779/154843703-4063dffe-d014-4b48-8f84-e96ebafe5a8f.png)
### Per sortir és donant a la tecla “esc” i després per guardar i sortir és “:wq”
### Després fem el mateix en l’ altre targeta de xarxa:
![image](https://user-images.githubusercontent.com/99834779/154843682-40d78389-3657-4f56-96d7-a6e82060b87a.png)
### Dintre ha d’ estar així, per modifcar les coses de dintre és donant a la tecla “i”:
![image](https://user-images.githubusercontent.com/99834779/154843674-324f8cbc-dfd9-4f82-a29c-437cdb952b5c.png)
### Per sortir és donant a la tecla “esc” i després guardar i sortir és “:wq”
### Després posem aquesta comanda per reiniciar el servei d’ internet:
![image](https://user-images.githubusercontent.com/99834779/154843671-f09559c2-8ab8-491c-a46e-43d00b14833c.png)
### Després mirem el seu estat:
![image](https://user-images.githubusercontent.com/99834779/154843657-71b97e28-c6a5-465f-96f2-1c445fc627ad.png)
### Ara mirem les connexions com han quedat:
![image](https://user-images.githubusercontent.com/99834779/154843649-fcb7512b-628f-47e6-831d-d731fa9b9e3a.png)
### Ara posem l’ update i upgrade  i és amb aquesta comanda:
![image](https://user-images.githubusercontent.com/99834779/154843647-76c4437d-cc38-4ddd-a43f-c8510c1d5f21.png)
![image](https://user-images.githubusercontent.com/99834779/154843640-9f2dfcc7-a467-4493-b2a2-d53456010e27.png)
### Ara instal•lem el repositori de percona:
![image](https://user-images.githubusercontent.com/99834779/154843635-338b8d2d-240a-455d-b2ac-822e89c04ec1.png)
### Després habiltem el percona server:
![image](https://user-images.githubusercontent.com/99834779/154843632-fbcd5583-8aa3-487a-bccc-f22c7cdcac2a.png)
### Ara instal•lem el Percona Server:
![image](https://user-images.githubusercontent.com/99834779/154843627-2c1279ea-f647-4fce-9ec3-c545ac6c9471.png)
### Ara inicem el mysql server:
![image](https://user-images.githubusercontent.com/99834779/154843622-85229068-99f0-4e4e-8d9b-ee43c6f7847b.png)
### I per últim mirem el seu estat:
![image](https://user-images.githubusercontent.com/99834779/154843575-cc807258-f6a4-4766-a1b9-1893f187cb30.png)
### Ara per mirar si funciona entrem dintre del mysl:
![image](https://user-images.githubusercontent.com/99834779/154843568-f7442463-6aba-46d7-b2c1-4e4135bcbc64.png)
