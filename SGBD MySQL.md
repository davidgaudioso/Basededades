### Part II - INSTAL•LACIÓ SGBD MySQL 8.0 (màx. 2 punt) 
![image](https://user-images.githubusercontent.com/99834779/154859057-1833be34-0ed0-44c9-9024-029593563ec0.png)

 
### ENUNCIAT  
 
### Partint d'una màquina CentOS 7 minimal proporcionada pel professor realitza la instal•lació d'un SGBD MySQL. Concretament la versió 8.0. 
 
### Notes 
### •	La màquina de la part I i la part II han de ser diferents. 
### •	No s'ha d'intal•lar MariaDB!!! 
 
### ENLLAÇOS 
 
 
### Fitxer codi font MySQL 8.0 (Generic Linux)  
 ### https://dev.mysql.com/doc/refman/8.0/en 
 
 
### LLIURAMENT 
 
### Pots utilitzar aquest document com a plantilla per el lliurament de l’activitat, inclou la webgrafia utilitzada per la realització de l’activitat. 
 
### Altres opcions de lliurament: 
### •	Utilitzar aquest document com a plantilla per el lliurament de l’activitat i penjar-la en tasca destinada a aquesta activitat dins del curs Moodle  
### •	Realitzar la documentació sobre un repositori GIT. Utilitzant el format de fitxer 
### MarkDown (MD). (1 punt) 
### •	Dins d'una WikiMedia. (1 punt) 
 
 
### REALITZA LA DOCUMENTACIÓ NECESSÀRIA PER LA INSTAL•LACIÓ PAS A PAS. 
 
### •	Indica clarament els passos per reproduir la instal•lació en un altra màquina. 
 
### •	Si realitzes algun canvi en la configuració del firewall, o altres elements de seguretat per poder tenir accés indica quins canvis has hagut de fer. 
 
### •	Cal tenir en compte que la documentació va dirigida a tècnics informàtics i no a usuaris no experts. 
 
### •	Es valorarà la presentació, l'organització del text i la facilitat de lectura. 

### Primer instal•lem un Centos 7 com en l’anterior exercici.
### Després configurem els dos fitxers de xarxa, per entrar al fitxer de xarxa enp0s3:
![image](https://user-images.githubusercontent.com/99834779/154859041-05f6ecf4-e13c-4471-a30c-27d00c1eccaf.png)
### Dintre ha d’ estar així, per modifcar les coses de dintre és donant a la tecla “i”:
![image](https://user-images.githubusercontent.com/99834779/154859037-3d551eec-12ce-4a8a-82e6-69b02b3afb2c.png)
### Per sortir és donant a la tecla “esc” i després per guardar i sortir és “:wq”
### Després fem el mateix en l’ altre targeta de xarxa:
![image](https://user-images.githubusercontent.com/99834779/154859007-b5035c63-ca87-4f15-b6ef-b4a4c5f19480.png)
### Dintre ha d’ estar així, per modifcar les coses de dintre és donant a la tecla “i”:
![image](https://user-images.githubusercontent.com/99834779/154859000-6c9e8446-f0da-4561-be80-a4c04133e302.png)
### Per sortir és donant a la tecla “esc” i després guardar i sortir és “:wq”
### Després posem aquesta comanda per reiniciar el servei d’ internet:
![image](https://user-images.githubusercontent.com/99834779/154858994-eabe17a3-f896-4c3b-9fc2-865d91e89353.png) 
### Després mirem el seu estat:
![image](https://user-images.githubusercontent.com/99834779/154858989-b9dfca6a-f865-46d7-a44d-2872ac2894d0.png)
### Ara mirem les connexions com han quedat:
![image](https://user-images.githubusercontent.com/99834779/154858982-5e9ab16e-9fd8-4526-a737-19d01a9815d0.png)
### Ara que tenim la xarxa instal•lada començarem a fer l’ instal•lació del SGBD MySQL:
### Primer fem un update i upgrade:
![image](https://user-images.githubusercontent.com/99834779/154858970-595739a8-31ca-4175-8e03-ee0d7a7d9fc4.png)

![image](https://user-images.githubusercontent.com/99834779/154858964-aa926ef6-e236-409b-8d92-5235845a08ba.png) 
### Després descarreguem el repositori de MySQL i el descarreguem dintre del directori /tmp:
![image](https://user-images.githubusercontent.com/99834779/154858961-111460e7-c056-4854-b8ea-e0f23f6772f0.png)
### Ara amb aquesta comanda instal•larem el repositori abans descarregat:
![image](https://user-images.githubusercontent.com/99834779/154858959-e5117e42-06aa-4896-bf4f-234a5008124c.png)
### Després instal•lem el MySQL:
![image](https://user-images.githubusercontent.com/99834779/154858955-747c2921-6db3-4354-9931-cef45c332757.png)
### Després de instal•lar el servei  l’ iniciarem i mirarem el seu estat:
![image](https://user-images.githubusercontent.com/99834779/154858944-4e7b3a9c-ddcf-43c1-bb89-119d798f4a61.png)
![image](https://user-images.githubusercontent.com/99834779/154858929-82676d9f-1dc6-4dcc-8f39-5e30aece11e5.png)
### Després comprovem la versió que hem instal•lat:
![image](https://user-images.githubusercontent.com/99834779/154858921-4965d36b-a9b6-4fd1-bd1d-161c10043a01.png)
### Ara per comprobar de connectar-nos el MySQL per defecte genera una contrasenya per l’usuari root per esbrinar-la será amb aquesta comanda:
![image](https://user-images.githubusercontent.com/99834779/154858915-08d8252c-8ecd-48fe-968f-002dd1f3e40c.png)
### En el nostre cas canviarem la contraseya i es fara amb aquesta comanda, en demanara la nova contrasenya:
![image](https://user-images.githubusercontent.com/99834779/154858906-020cc143-a120-481e-82c3-85bb974ae795.png) 
![image](https://user-images.githubusercontent.com/99834779/154858902-b34f4a09-9894-4157-8b6f-ff5d3e3adfc1.png)
![image](https://user-images.githubusercontent.com/99834779/154858895-c47a1e8b-77bd-427c-8189-950a17a1e8da.png)
![image](https://user-images.githubusercontent.com/99834779/154858884-5a6094fa-8004-4550-9b7d-e0d4f0582d35.png)
![image](https://user-images.githubusercontent.com/99834779/154858876-4b1c036f-6396-43bc-93dd-ed2132223708.png)
### Ara comprovem si podem entrar dintre del MySQL amb la nova contrasenya:
![image](https://user-images.githubusercontent.com/99834779/154858866-b4cf4b73-d298-4b6f-b2dd-b56af3941ffc.png)
### Després en el meu cas li he canviat un altre cop la contrasenya perque sigui “patata” i per aixó he de canviar els permisos de contrasenyes de MySQL i es d’aquesta manera:
![image](https://user-images.githubusercontent.com/99834779/154858862-373ac618-d8c5-4d80-87dd-db643287e5ad.png)
### I per últim comprovem si podem entrar dintre amb la nova contrasenya:
![image](https://user-images.githubusercontent.com/99834779/154858853-4fa52ba0-bb24-4342-bddc-012a1a90d5b7.png)
 
### RESPON O COMPROVA ELS SEGÜENTS APARTATS 

### 1.	A on es troben físicament els fitxers de dades? 
![image](https://user-images.githubusercontent.com/99834779/154858846-b35abe39-6381-4902-bd51-ce75b25b7904.png)
### 2.	A on es troba el fitxer de configuració? Quin és el seu contingut? 
### Aquet fitxer es trova en la ubicació /etc i l’ arxiu es diu així i té aquest contingut:
![image](https://user-images.githubusercontent.com/99834779/154858834-fd9e37f3-04e8-44f5-b06b-62c9b0c45380.png)
### 3.	El procés de mysqld escolta al port 3306. Quina modificació/passos caldrien fer per canviar aquest port a 33306 per exemple? Important: No realitzis els canvis. Només indica els passos que faries. 
### Per canviar el port haurem de posar aquesta comanda i posem el port 33306:
![image](https://user-images.githubusercontent.com/99834779/154858830-269114f1-fca1-4a7e-b516-de59ef454363.png)
### Després haurem de reiniciar el firewall per que s’apliquen els canvis:
![image](https://user-images.githubusercontent.com/99834779/154858827-b43b4f8f-ef02-46e5-83f8-116239f80f0c.png)
### 4.	Un cop finalitzada la instal•lació i veure que funciona, mostra el resultat de la comanda:  
### ps -ef | grep mysql 
![image](https://user-images.githubusercontent.com/99834779/154858821-04d07a2e-104d-4f79-ad9c-8af3f678577c.png)
### 5.	Quines són les característiques principals que ofereix MySQL 8.0 enfront de la 5.7. 
### Les característiques prinicipals que he vist son que amb la versió de MySQL 8.0 el rendiment augmenta com per exemple en la carrega de lectura o escriptura, un altre cosa que també ha millorat es la funció de emmagatzematge de NoSQL, també a partir de la versio 8.0 s'ha afegit un nou concepte anomenat funció de finestra, que es pot fer servir per implementar diversos mètodes de consulta nous. També proporciona suport per ordenar índexs en ordre descendent.
### 6.	Ensenya al professor que us podeu connectar al SGBD. 
### Per poder conectar al SGBD he creat un usuari i es crearía d’aquesta manera:
![image](https://user-images.githubusercontent.com/99834779/154862918-90265e7c-e3ed-4aea-92ac-002e79b49886.png)
![image](https://user-images.githubusercontent.com/99834779/154858806-ba21eee3-6fb9-4ad4-9a94-bbe5f4b1e829.png) 
### I també he d’activar el port 3306 i és amb aquesta  comanda:
![image](https://user-images.githubusercontent.com/99834779/154858799-f2dbf478-62df-4640-816f-b76d2cd156f7.png)
### Després haurem de reiniciar el firewall perque s’apliquen els canvis:
![image](https://user-images.githubusercontent.com/99834779/154858784-dab9c490-3f51-4601-806e-1fb90806b152.png)
### Després he anat al workwench i he creat una connexió amb el port que és 3306 i posant l’ usuari que he creat abans:
![image](https://user-images.githubusercontent.com/99834779/154858778-d5cab4fd-9dec-4950-9202-e65d4a3cc694.png)
### I ens connectem:
![image](https://user-images.githubusercontent.com/99834779/154858774-4ddba168-024f-41bc-9231-d7614612f013.png)
