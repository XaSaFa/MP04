# Activitat 1 - Compartir recursos entre servidor Linux i Windows 10 utilitzant NFS

Entregueu un pdf amb el resultat de la següent activitat.

Per a fer aquesta activitat utilitzaràs un Servidor Linux i un client Windows 10 a la mateixa xarxa (ISARD).

## IP Linux: 192.168.1.100

![image](https://github.com/user-attachments/assets/4d0629bf-4c27-4d01-a53b-28dd14ea5431)

![image](https://github.com/user-attachments/assets/7ba5483f-653b-4292-9b1c-2189557b3061)


## IP Windows: 192.168.1.200

![image](https://github.com/user-attachments/assets/ac43a6be-d60d-4003-b1b1-039674de73be)


1. Crea la carpeta "/general" a Linux i comparteix-la (canvia permisos i propietari i edita el fitxer /etc/exports).

![image](https://github.com/user-attachments/assets/81ea63e4-e1e6-4d88-ab8e-f8bbd5d30161)

2. Comprova que tens accés des de Windows a la carpeta.
4. Munta la carpeta anterior a la unitat K del client.
5. Fes que la carpeta es munti automàticament quan es reiniciï l'ordinador client.
6. Crea alguns fitxers a la carpeta.
7. Programa una còpia de seguretat diaria al servidor Linux de la carpeta /general.
8. Esborra els fitxers de la carpeta general des del client Windows.
9. Recupera la còpia de seguretat des de Linux i deixa la carpeta com estava.
