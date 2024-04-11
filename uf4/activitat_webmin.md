# Utilitzant webmin per administrar el servidor

## 1.- Crear i modificar usuaris

- Has de crear dos usuaris user1_X i user2_X on (X és el vostre cognom).
- Els usuaris et passaran el hash de la seva contrasenya, no la contrasenya real. (podeu fer servir openssl).
- Cada usuari tindrè un directori a home igual al seu nom d'usuari.
- Utilitzaran bash com a shell.
- Els usuaris estaran dins del grup que tingui el seu mateix nom i dins del grup usuaris_empresa.
- L'usuari user2_X no podrà fer login després del dia 21-04-2024.
- Comproveu que els usuaris poden iniciar sessió.
- Canvia la data del sistema (utilitzant webmin) i comprova que user2_X no pot iniciar sessió si estem a dia 22-04-2024.

## 2.- Programa tasques

- Programa una tasca que neteja els paquets de Linux que ja no s'utilitzen una vegada al mes.
- Programa una còpia de seguretat diària del directori home dels usuaris a /srv/backup.
- Crea fitxers, fes que s'executi la tasca programada i comprova que es pot recuperar la informació (fora de webmin). 

## 3.- Instal·lació de software

- Utilitza webmin per mostrar quins paquets de software es podrien actualitzar.
- Des de webmin actualitza un paquet.
- Utilitza webmin per instal·lar un joc de apt.
- Utilitza webmin per instal·lar gimp de apt.
- Utilitza webmin per desinatl·lar el joc que heu instal·lat abans.

## 4.- Serveis

- Utilitza webmin per mostrar els serveis que s'inicien amb el sistema.
- Utilitza webmin per mostrar els serveis que estan actius.
- Utilitza webmin per mostrar l'estat del servidor Apache.
- Utilitza webmin per aturar Apache.
- Utilitza webmin per mostrar l'estat del servidor Apache.
- Utilitza webmin per reiniciar Apache.
- Utilitza webmin per mostrar l'estat del servidor Apache.

## 5.- Quotes de disc

Activa les quotes de disc pels usuaris ammb la comanda: 

```
sudo apt install quota quotatool
```

- Utilitza webmin perquè l'usuari user1_X no pugui tenir més de 2 MB d'informació al disc.
- Comprova que la quota funciona.
- Utilitza webmin perquè l'usuari user2_X no pugui tenir més de 10 fitxers al disc.
- Comprova que la quota funciona.
