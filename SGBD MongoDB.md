### PART III - INSTAL•LACIÓ SGBD MongoDB (màx. 1 punt) 
![image](https://user-images.githubusercontent.com/99834779/154859424-d250ddfe-1436-4c2c-8725-6b310c9c4159.png)

  
### ENUNCIAT  
 
### Partint d'una màquina CentOS 7 minimal proporcionada pel professor realitza la instal•lació d'un SGBD NoSQL MongoDB (última versió). 
 
### Nota: La màquina de la part I i la part II han de ser diferents. 
 
### ENLLAÇOS 
 
 
### Documentació oficial d’instal•lació  MongoDB  	https://docs.mongodb.com/manual/installation/ 
 
### LLIURAMENT 
 
### Pots utilitzar aquest document com a plantilla per el lliurament de l’activitat, inclou la webgrafia utilitzada per la realització de l’activitat. 
 
### Opcions d'entrega: 
### •	Utilitzar aquest document com a plantilla per el lliurament de l’activitat i penjar-la en tasca destinada a aquesta activitat dins del curs Moodle  
### •	Realitzar la documentació sobre un repositori GIT. Utilitzant el format de fitxer MarkDown (MD). (1 punt) 
### •	Dins d'una WikiMedia. (1 punt) 
 
 
### REALITZA LA DOCUMENTACIÓ NECESSÀRIA PER LA INSTAL•LACIÓ PAS A PAS. 
 
### •	Indica clarament els passos per reproduir la instal•lació en un altra màquina. 
 
### •	Si realitzes algun canvi en la configuració del firewall, o altres elements de seguretat per pode tenir accés indica quins canvis has hagut de fer. 
 
### •	Cal tenir en compte que la documentació va dirigida a tècnics informàtics i no a usuaris no experts. 
 
### •	Es valorarà la presentació, l'organització del text i la facilitat de lectura. 
 
### •	Incloure en la documentació un petit apartat a on s'expliqui com realitzar la connexió a la BD. 
 
### •	Ensenya al professor que us podeu connectar al SGBD. 
 








### Primer instal•lem un Centos 7 com en els dos anteriors exercicis.
### Després configurem els dos fitxers de xarxa, per entrar al fitxer de xarxaa enp0s3:
![image](https://user-images.githubusercontent.com/99834779/154859417-a3525fad-7062-4884-85f1-e7dcd737d814.png)
### Dintre ha d’ estar així, per modifcar les coses de dintre és donant a la tecla “i”:
![image](https://user-images.githubusercontent.com/99834779/154862991-120fe2b9-9c82-4359-b399-66231ffc39c2.png)
### Per sortir és donant a la tecla “esc” i després per guardar i sortir és “:wq”
### Després fem el mateix en l’ altre targeta de xarxa:
![image](https://user-images.githubusercontent.com/99834779/154859396-3cc016fa-301c-4016-ac65-f8ce86b1f851.png)
### Dintre ha d’ estar així, per modifcar les coses de dintre és donant a la tecla “i”:
![image](https://user-images.githubusercontent.com/99834779/154863012-d2e15b5e-ef5d-4ae0-8edb-7d0eac7007f9.png)
### Per sortir és donant a la tecla “esc” i després guardar i sortir és “:wq”
### Després posem aquesta comanda per reiniciar el servei d’ internet:
![image](https://user-images.githubusercontent.com/99834779/154859387-409ffb62-18bb-4b36-a6fb-ac9e0d1c448e.png)
### Després mirem el seu estat:
![image](https://user-images.githubusercontent.com/99834779/154859381-47448b8d-c0b0-45bc-bb1c-5736d9984e64.png)
### Ara mirem les connexions com han quedat:
![image](https://user-images.githubusercontent.com/99834779/154859376-06841120-943b-4ac1-93ba-9858f4466789.png)
### Ara que tenim la xarxa instal•lada començarem a fer la instal•lació del MongoDB:
### Primer fem un update i upgrade:
![image](https://user-images.githubusercontent.com/99834779/154859331-c978eb9b-c9d2-4f03-a146-f8f9719685ec.png)
![image](https://user-images.githubusercontent.com/99834779/154859329-433148bd-30e2-467d-87c4-345bfcf3b821.png)
### Després de haber comfigurat la xarxa i actualitzar el Centos 7 començarem l’instal•lacio, primer crearem un arxiu de repositori:
![image](https://user-images.githubusercontent.com/99834779/154859325-0e84ddf7-63db-4961-b163-7dac2211a346.png)

### I té aquest contingut:
![image](https://user-images.githubusercontent.com/99834779/154859316-46aac94c-538c-4539-b92d-6d05710a782b.png)
### Després instal•larem el MongoDB amb la comanda següent:
![image](https://user-images.githubusercontent.com/99834779/154859306-bc863c82-2ea2-48c0-9019-e9e6036bc0f2.png)
### Ara iniciarem el servei de MongoDB:
![image](https://user-images.githubusercontent.com/99834779/154859299-79908744-ae4b-45d0-b74b-cf7ed484508d.png)
### Per acabar l’instal•lació mirarem el seu estat:
![image](https://user-images.githubusercontent.com/99834779/154859292-0af71ad8-585c-47c4-993c-8740f041f493.png)
### Per últim  mirarem si ens podem connectar a MongoDB:
![image](https://user-images.githubusercontent.com/99834779/154859280-ac7817ed-6ed0-41e4-aab0-982f3672efe8.png)
### Ara haurem de fer la seva configuració i anirem a modifcar l’arxiu amb aquest nom:
![image](https://user-images.githubusercontent.com/99834779/154859268-4662869e-b87f-4213-9b98-3cfa0a1728ce.png)
### I modifcarem les linies de “network interfaces”, la de “seucrity” i haura de quedar d’aquesta manera:
![image](https://user-images.githubusercontent.com/99834779/154859264-3b7b460a-eccb-435d-b849-2ada8c7b6226.png)
### Després reinciarem el servei:
![image](https://user-images.githubusercontent.com/99834779/154859259-2d37e442-d432-40af-8364-ca74c46d26b7.png)
### Ara entrem i crearem un usuari que en el meu cas es diu “david” per connectarnos remotament:
![image](https://user-images.githubusercontent.com/99834779/154859250-9b31f6a6-ea3f-4b2a-85b1-dd77b69eb74c.png)
![image](https://user-images.githubusercontent.com/99834779/154859246-a1c22278-2b3b-4c09-b54a-56df699f6857.png)
### I per comprovar que està bé creat entrarem a mongo amb ell:
![image](https://user-images.githubusercontent.com/99834779/154859242-04300ef3-73e7-4d5d-87d5-c08cfd05e5fd.png)

### Ara per poder conectarnos remotament a MongoDB configurarem el firewall i es d’aquesta manera:
![image](https://user-images.githubusercontent.com/99834779/154859233-989eed19-a1a7-4edf-bea3-78a3c0daa5a4.png)
### I també reiniciarem el servei:
![image](https://user-images.githubusercontent.com/99834779/154859222-6a85c100-3f4c-4db8-940e-6796af1c8e67.png)
### Després en el meu cas per conectarem remotament he utilitzat l’aplicacio “Robo 3T” i he creat una connexió nova amb aquesta configuració:
![image](https://user-images.githubusercontent.com/99834779/154859205-3fe6fa51-51e2-4043-b765-d18e0fa1c86d.png)![image](https://user-images.githubusercontent.com/99834779/154859208-569d4a91-c053-4f77-b4bb-91dd25ff9c7e.png)

### I li donarem després a conectar i ja estarem connectacts remotamnet  a MongoDB:
![image](https://user-images.githubusercontent.com/99834779/154859197-724e5871-2955-4d63-83e6-bbd168cce8ec.png)
