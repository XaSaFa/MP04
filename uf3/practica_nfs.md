# Pràctica NFS

L'objectiu d'aquesta pràctica és aplicar la compartició de fitxers NFS sobre equips en Linux.

## Usuaris

Tenim dos usuaris anomenats granota i ornitorinc, amb la següent informació:

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

Crearem una carpeta per cada usuari (granota i ornitorinc dins de zoo) les quals seran propietat del seu respectiu usuari.

![image](https://github.com/user-attachments/assets/0cef9ed2-a46c-4998-9358-286cc9740c85)

## Muntar la carpeta compartida al client

Crearem a l'ordinador client una carpeta a /mnt anomenada zoo, aquesta carpeta no tindrà propietari i tendrà tots els permisos habilitats

![image](https://github.com/user-attachments/assets/2835fd14-748a-41bb-877c-4313bb4eb883)

Aqui muntarem la carpeta /zoo del servidor i farem que es munti automàticament en encendre l'equip.

![image](https://github.com/user-attachments/assets/e59d5915-3df8-4864-b670-39b64b6aeaee)

![image](https://github.com/user-attachments/assets/46ce8992-93b8-4f3c-94ac-3b037aaf4b1e)

## Canviar el directori home dels usuaris a un directori del servidor.

Ara farem que el directori home dels usuaris creats granota i ornitorinc canviï, de /home/granota passarem a /mnt/zoo/granota i farem el mateix amb els directoris necessaris per a l'altre usuari.

Això ho aconseguim amb la comanda usermod i el paràmetre -d.

![image](https://github.com/user-attachments/assets/2798d3c7-95f1-4925-b3a2-105d0d5421b1)

Per tal de provar si funciona iniciarem sessió amb l'usuari granota a l'ordinador client.

Al fer-ho veurem que estem fent servir com a home de l'usuari la carpeta compartida per NFS.

![image](https://github.com/user-attachments/assets/63dec708-decb-41e7-b2ac-78deeaaeca96)

A més al servidor s'hauran creat les carpetes de l'usuari a /zoo/granota.

![image](https://github.com/user-attachments/assets/75912690-e3c9-41d7-9fbf-e49706822f24)

## Quina utilitat té aquesta utilització de NFS.
## Podria ser contraproduent en algun sentit?

## Ampliació

Feu la mateixa pràctica per a l'usuari cocodril, però feu que al server tingui un uid d'usuari de 1070 i al client de 1080.

Com afecta això al funcionament de NFS? Perquè deu ser?
