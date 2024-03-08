# Compartir carpeta home al server

# Pas 1.- Compartir la carpeta home

Per a fer-ho editem l'arxiu /etc/exports del servidor i afegim la línia següent:

```
/home *(rw,sync,no_root_squash,no_subtree_check)
```

![image](https://github.com/XaSaFa/MP04/assets/110727546/c8399c05-68e6-4db0-8056-4cbc790a42b7)

Reiniciem el servidor NFS:

```
sudo service nfs-kernel-server restart
```

# Pas 2.- Creem punt de muntatge al client

Dins l'ordinador client creem un punt de muntatge i canviem els permisos:

```
sudo mkdir -p /mnt/nfs/home
sudo chmod -R 777 /mnt/nfs/home
```

# Pas 3.- Muntem la carpeta del server al client

Muntem la carpeta home del servidor a la carpeta que hem creat al client. Des de l'ordinador client escrivim la comanda:

```
sudo mount 192.168.1.10:/home /mnt/nfs/home
```

![image](https://github.com/XaSaFa/MP04/assets/110727546/4a591348-b7db-4fb8-a45d-4620f0677559)

# Pas 4.- Utilitzem la carpeta home

Anem a /mnt/nfs/home/usuari i creem algun fitxer

![image](https://github.com/XaSaFa/MP04/assets/110727546/0f5b218c-b959-41ab-a736-4dc627cd9bd7)

# Pas 5.- Fem que el muntatge sigui permanent

Quan reiniciem l'equip es perdra el muntatge, per fer-ho permanent anem a editar /etc/fstab i afegir la següent línia:

```
192.168.1.10:/home /mnt/nfs/home nfs auto,noatime,nolock,bg,nfsvers=3,intr,tcp,actimeo=1800 0 0
```

![image](https://github.com/XaSaFa/MP04/assets/110727546/acac528e-5327-47d6-a784-4765ab3d31ee)



🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎

Activitat:

Per probar com funciona el muntatge de /home fes aquesta activitat:

1. Segueix el tutorial.
2. Al client crea un usuari anomenat alumne_X on X és el teu cognom i inicia sessió.
3. Al client prova a escriure a la carpeta /mnt/nfs/home d'altres usuaris.
4. Al servidor crea el mateix usuari alumne_X.
5. Al client prova a escriure a la carpeta /mnt/nfs/home de l'usuari alumne_X des del compte d'alumne_X.
6. Quines conclusions en treus?

🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎🔎
