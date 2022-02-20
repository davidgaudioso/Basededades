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
![image](https://user-images.githubusercontent.com/99834779/154862677-96318a85-6099-4955-9109-40e353f1fe4c.png)
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

### RESPON O COMPROVA ELS SEGÜENTS APARTATS 
 
### 1.	Un cop realitzada la instal•lació realitza una securització de la mateixa. Quin programa realitza aquesta tasca? Realitza una securització de la instal•lació indicant que la contrasenya de root sigui patata. 
### Per canviar la contrasenya primer he mirat la contrasenya que té per defecte i és amb aquesta comanda:
![image](https://user-images.githubusercontent.com/99834779/154858495-00765147-fcdf-471e-8b8f-15eeffbc5094.png)
### Després entrem dintre del mysql amb la contrasenya que té per defecte:
![image](https://user-images.githubusercontent.com/99834779/154858501-af874527-dc16-491c-bdf1-44559c423306.png)
### Ara dintre del mysql poso aquestes comandes per canviar els permisos de les contrasenyes del mysql i faig això perqué sino no hem deixa posar “patata” de contrasneya:
![image](https://user-images.githubusercontent.com/99834779/154858507-fb4af746-eac0-4d78-a216-220235f61cf5.png)
![image](https://user-images.githubusercontent.com/99834779/154858510-9ec4d52b-ce56-45b4-a294-f162a0c3d960.png)
### Després de canviar els permisos canviem la contranseya del usuari root:
![image](https://user-images.githubusercontent.com/99834779/154858514-1cf367f3-479e-40a0-9ff7-07aa7a9c4ac1.png)
### Per mirar si funciona sortirm del mysql i tornen a entrar pero posant la nova contrasenya:
![image](https://user-images.githubusercontent.com/99834779/154858520-f32a7073-917d-4a8f-876f-14c6b88b7a85.png)
### 2.	Quines són les instruccions per arrancar / verificar status / apagar servei de la base de dades de Percona Server en el CentOS 7 
### Per arrancar el servei:
![image](https://user-images.githubusercontent.com/99834779/154858524-fe14a3dd-907b-4444-8e72-997e6b18eab0.png)
### Per verificar status el servei:
![image](https://user-images.githubusercontent.com/99834779/154858528-7199a0ee-cfed-49ec-98c8-3f0668dbb21e.png)
### Per apagar el servei:
![image](https://user-images.githubusercontent.com/99834779/154858532-d372b8df-2b09-4c99-973a-c324a9458078.png)
### 3.	A on es troba i quin nom rep el fitxer de configuració del SGBD Percona Server? 
### L’ arxiu de configuració té aquest nom i està ubicat en /etc/my.cnf i té aquest contingut:
![image](https://user-images.githubusercontent.com/99834779/154858538-43f2873e-b499-48b5-b032-43eff9a53ffe.png)
### 4.	A on es troben físicament els fitxers de dades (per defecte). Com ho has sabut? 
### L’ arxiu on es troben físicament els fitxers de dades per defecte es en la ubicació /var/lib/mysql i ho he descobert perqué està en l’ arxiu de configuració:
![image](https://user-images.githubusercontent.com/99834779/154858544-99f2ebb8-3a22-43d1-ab2a-d3057df163d0.png) 
### 5.	Crea un usuari anomenat asix en el sistema operatiu i en SGBD de tal manera que aquest usuari del sistema operatiu no hagi d'introduir l'usuari i password cada vegada que cridem al client mysql? 
### i.	https://dev.mysql.com/doc/refman/8.0/en/password-security-user.html 
### ii.	Usuari SO-→ asix / patata iii. Usuari MySQL → asix / patata 
### Primer creem l’ usuari del SO i és amb aquestes comandes la primera per crear l’ usuari i la segona per posar-li contrasenya:
![image](https://user-images.githubusercontent.com/99834779/154858553-a1f109f5-c283-4572-a9ec-d1c22e55376a.png)
### Després creem l’ usuari de MySQL:
### Primer canviem els permisos de contrasenyes del MySQL i és amb aquestes comandes:
![image](https://user-images.githubusercontent.com/99834779/154858560-572226b5-cd6f-47df-8b9b-7e1adc729a6f.png)
![image](https://user-images.githubusercontent.com/99834779/154858565-a17e1c33-9113-4950-b7ab-3e36712619a4.png)
![image](https://user-images.githubusercontent.com/99834779/154858568-0ca35b5a-4e06-41bc-bf86-3938c089b736.png)
### Després creem l’ usuari i li posem permisos perqué pugui consultar,modifcar,esborrar les	dades de les bases de dades:
![image](https://user-images.githubusercontent.com/99834779/154858575-959d35ab-2ba6-4787-a697-8a5d9c286b1e.png)
![image](https://user-images.githubusercontent.com/99834779/154858580-92369ab2-2454-4ad7-9c29-cb96e515fdfe.png)
### Ara fem la cofiguració perque no demani la contrasenya quant inici sessio a MySQL i primer hem de configurar aquest arxiu:
![image](https://user-images.githubusercontent.com/99834779/154858584-9c882df3-60a6-4aed-833a-6bd60d8447ff.png)
### I dintre posem aquesta configuració:
![image](https://user-images.githubusercontent.com/99834779/154858590-72c43c8d-9bbc-4fbf-b06e-5f7c981a810f.png) 
### Ara inciem amb l’ usuari asix i ho comprovem:
![image](https://user-images.githubusercontent.com/99834779/154858599-786981f8-9b06-4e1a-8c76-4c475008d780.png)
### 6.	El servei de MySQL (mysqld) escolta al port 3306. Quina modificació/passos caldrien fer per canviar aquest port a 33306 per exemple?  
### Per canviar el port haure de posar aquesta comanda i posem el port 33306:
![image](https://user-images.githubusercontent.com/99834779/154858613-61f45c10-e9a3-442c-aa18-934af2b881ab.png)
### Després haurem de reiniciar el firewall perque s’apliquen els canvis:
![image](https://user-images.githubusercontent.com/99834779/154858622-c9886b94-f62f-472b-9618-9eb69a7eb376.png)
### 7.	Important: No realitzis els canvis. Només indica els passos que faries. 
 	
### 8.	Ensenya al professor que us podeu connectar al SGBD. 
### Per fer la prova de conectarme he utilitzat el programa workbench, en aquest programa he creat aquesta connexió:
![image](https://user-images.githubusercontent.com/99834779/154858627-1937f951-a71d-461d-90fa-48034b78d432.png)
### Quant estem dintre he fet un select per comprovar que funciona:
![image](https://user-images.githubusercontent.com/99834779/154858633-99d1fad5-6195-49f4-9c2b-c540244e4ea5.png)

