# Compartir una carpeta al grup de treball des de Linux

Ja hem vist com compartir una carpeta des de Windows al grup de treball, però ara ho farem des d'un ordinador amb Linux instal·lat.

## Pas 1.- Crear una carpeta per compartir

Com exemple a la carpeta personal de l'usuari de Linux creem una carpeta anomenada "documents_de_grup".

![image](https://github.com/XaSaFa/MP04/assets/110727546/c88e5b35-de99-4c26-8d77-0e2b8e9c73ed)

## Pas 2.- Compartir la carpeta

Pressionem botó dret i seleccionem "Propiedades".

![image](https://github.com/XaSaFa/MP04/assets/110727546/53e3c5c1-71e2-43a5-842d-0b3cd57a8b10)

Anem a la pestanya "Recurso compartido de red local".

![image](https://github.com/XaSaFa/MP04/assets/110727546/385de1f8-f611-42cf-984a-593835e33375)

Seleccionem la casella "Compartir esta carpeta", si és la primera vegada que ho fem Linux ens avisa que ha d'instal·lar software addicional.

![image](https://github.com/XaSaFa/MP04/assets/110727546/3c4e8aad-d684-4697-8856-a7bf9025e71f)

Instal·lem el servei SAMBA com ens proposa Linux.

![image](https://github.com/XaSaFa/MP04/assets/110727546/eec0e522-3736-4d08-b98a-77ac05523acc)

![image](https://github.com/XaSaFa/MP04/assets/110727546/7a35410e-06e9-4e47-ad47-ba1cb314ecb9)

Ens demanarà credencials d'admin i començarà a instal·lar-se el servei.

## Pas 3.- Seleccionar accés de només lectura o lectura i modificació

Quan compartim la carpeta Linux hem d'escollir si la compartim només amb permisos de lectura o amb permisos per llegir i modificar, per això hem de seleccionar següent la casella en el segon cas.

![image](https://github.com/XaSaFa/MP04/assets/110727546/3f6aa992-e6ee-463d-a10e-7ca9098c735c)

Seleccionem "Crear compartición".

![image](https://github.com/XaSaFa/MP04/assets/110727546/68bbff78-793e-4d0b-8900-8a33c1b8b695)

El sistema ens avisa que el nom del recurs a compartir és massa llarg així que el fem més curt.

![image](https://github.com/XaSaFa/MP04/assets/110727546/7a573e7f-59d7-4d7d-bddb-19f3120f62e8)

Si hem modificat els permisos per a que els usuaris puguin modificar fitxers Linux ens avisarà de que ha de fer modificacions als permisos de la carpeta.

![image](https://github.com/XaSaFa/MP04/assets/110727546/621ee5eb-72f5-4a41-b52b-c26fa7536271)

Com veiem l'icona de la carpeta compartida ha canviat.

![image](https://github.com/XaSaFa/MP04/assets/110727546/fa89abdd-d8a0-4a9b-a3d4-dd972cc7a775)

Si obrim un terminal veurem com han quedat els permisos de la carpeta.

![image](https://github.com/XaSaFa/MP04/assets/110727546/927ab900-0c29-41f1-a1fd-c79c8fa154f5)

A Linux afegim un fitxer dins la carpeta compartida.

![image](https://github.com/XaSaFa/MP04/assets/110727546/c9a84a30-e781-4812-8392-b1e74c4d4c62)


