# Pràctica NFS

L'objectiu d'aquesta pràctica és aplicar la compartició de fitxers NFS sobre equips en Linux.

## Usuaris

Tenim dos usuaris anomenats granota i jaguar, amb la següent informació:

- Nom usuari: granota.
- UID: 1050

- Nom usuari: ornitorinc
- UID: 1060

![image](https://github.com/user-attachments/assets/4649c55a-d21f-48f7-a106-fafb130d6d14)

Per a assignar un nom d'usuari feu servir el paràmetre -u a la comanda adduser.

## Carpeta compartida per NFS

Hem de preparar al servidor un directori compartit anomenat /zoo que utilitzarem des del ordinador client

![image](https://github.com/user-attachments/assets/e4d0661d-80ea-4ebb-924b-5aa7d08762ec)

El compartim per lectura i escriptura.

## Muntar la carpeta compartida al client

Crearem a l'ordinador client una carpeta a /mnt anomenada zoo, aquesta carpeta no tindrà propietari i tendrà tots els permisos habilitats

![image](https://github.com/user-attachments/assets/2835fd14-748a-41bb-877c-4313bb4eb883)

Aqui muntarem la carpeta /zoo del servidor.

![image](https://github.com/user-attachments/assets/e59d5915-3df8-4864-b670-39b64b6aeaee)

També farem que la carpeta es munti automàticament en encendre l'equip.

## Còpies de seguretat

Per tal de guardar la informació dels usuaris creareu còpies de seguretat que es guardaran al server.

Heu de crear una carpeta compartida al server amb cada usuari. Les carpetes estaran dins del directori /zoo i cada usuari tindrà un subdirectori propi, per exemple l'usuari granota tindrà un directori anomenat /zoo/granota.

Programareu les còpies de seguretat per que es facin diariament per terminal ([apunts UF2](https://github.com/XaSaFa/MP04/blob/main/uf2/readme.md)).

Les còpies es guardaran en un format de compressió a la vostra elecció.

El nom de cada fitxer de còpia de seguretat tindrà la forma backup-nomusuari-dd-mm-aaaa-hh-mm seguit del punt i el format de fitxer.

## Directori home

Els usuaris fan servir 
