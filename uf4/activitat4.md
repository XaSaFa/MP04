# Activitat 4 - Compartir carpetes de Linux a Windows utilitzant SAMBA

# 1.- Carpeta sense autenticació:

- Crea una carpeta a la MV Linux a /srv/samba/compartida1 amb els permisos necessaris perquè pugui accedir tothom.
- Crea la configuració de SAMBA per compartir la carpeta per a convidats (sense autenticació) amb lectura i escriptura.
- Reinicia el servei SAMBA.
- Comprova que tens accés des de Windows.
- Crea algun fitxer a la carpeta.
- Comprova que s'ha creat a Linux.

# 2.- Carpeta per a usuaris determinats

- Crea una carpeta a la MV Linux a /srv/samba/compartida2 amb els permisos necessaris.
- Crea un usuari local anomenat user1_X (on X és el teu cognom).
- Afegeux l'usuari anterior a SAMBA.
- Crea la configuració de SAMBA per compartir la carpeta per a l'usuari anterior amb lectura i escriptura amb màscara de fitxers 755.
- Reinicia el servei SAMBA.
- Comprova que tens accés des de Windows amb les credencials de l'usuari.
- Crea algun fitxer a la carpeta.
- Comprova que s'ha creat a Linux i té els permisos 755.

# 3.- System-config-samba

- System-config-samba és una interfície gràfica per configurar recursos compartits utilitzant SAMBA.
- Investigar com instal·lar i utilitzar System-config-samba.
- Utilitzant System-config-samba:
  - Crea una carpeta a la MV Linux a /srv/samba/compartida3 amb els permisos necessaris.
  - Crea un usuari local anomenat user2_X (on X és el teu cognom).
  - Afegeix l'usuari anterior a SAMBA.
  - Crea la configuració de SAMBA per compartir la carpeta per a l'usuari anterior amb lectura i escriptura amb màscara de fitxers 744.
  - Reinicia el servei SAMBA.
  - Comprova que tens accés des de Windows amb les credencials de l'usuari.
  - Crea algun fitxer a la carpeta.
  - Comprova que s'ha creat a Linux i té els permisos 744.

