# UF3 - Compartició de recursos i seguretat

![image](https://github.com/XaSaFa/MP04/assets/110727546/1dcee92e-e0ca-46a9-9115-3c300955b547)

## Programació

- [Programació UF3](https://github.com/XaSaFa/MP04/blob/main/uf3/programacio.md)

## Permisos i drets

- [Permisos i drets](https://github.com/XaSaFa/MP04/blob/main/uf3/permisos_i_drets.md)

## Compartir recursos

### Windows

Per compartir recursos a Windows necessitem dues MV:
- Windows Server 2016.
- Windows 10.

- A Windows Server heu d'instal·lar active directory i crear un domini anomenat COGNOM.COM (aquí teniu enllaços a la teòria del tema 1):
  - [Instal·lar rol AD](https://github.com/XaSaFa/MP04/blob/main/uf1/instalar_domini.md).
  - [Promocionar el controlador de domini](https://github.com/XaSaFa/MP04/blob/main/uf1/instalar_domini2.md)
  - [Després heu d'unir el client al servidor](https://github.com/XaSaFa/MP04/blob/main/uf1/conectar_client_a_domini.md)

- Connectar unitats de xarxa i recursos de xarxa
  - [Net use](https://github.com/XaSaFa/MP04/blob/main/uf3/connectar_unitat_xarxa.md)
  - [Connectar a unitat de xarxa i recurs de xarxa de forma gràfica](https://github.com/XaSaFa/MP04/blob/main/uf3/connectar_unitat_xarxa_visual.md)
  - [Crear una carpeta personal per als usuaris del domini](https://github.com/XaSaFa/MP04/blob/main/uf3/carpeta_personal_windows.md)
  - [Compartir impressora](https://github.com/XaSaFa/MP04/blob/main/uf3/compartir_impressora.md)

- Directives de grup
  - [Crear una directiva de grup per una unitat organitzativa](https://github.com/XaSaFa/MP04/blob/main/uf3/directives.md)
 
### Linux

Per compartir recursos a Linux necessitem dues MV:
- Ubuntu 22.04LTS (Servidor).
- Linux Mint (client).

- NFS:
  - [Què és NFS](https://github.com/XaSaFa/MP04/blob/main/uf3/nfs0.md)
  - [Instal·lar NFS al server](https://github.com/XaSaFa/MP04/blob/main/uf3/nfs1.md)
  - [Instal·lar NFS al client](https://github.com/XaSaFa/MP04/blob/main/uf3/nfs2.md)
  - [Crear el recurs compartit](https://github.com/XaSaFa/MP04/blob/main/uf3/nfs3.md)
  - [Accedir a la carpeta compartida des d'un client](https://github.com/XaSaFa/MP04/blob/main/uf3/nfs4.md)
  - [Muntar automàticament les carpetes compartides](https://github.com/XaSaFa/MP04/blob/main/uf3/nfs5.md)
  - [Muntar la carpeta home del servidor per cada usuari client](https://github.com/XaSaFa/MP04/blob/main/uf3/practica_nfs.md)
  - [Compartir una impressora entre equips en xarxa Linux](https://github.com/XaSaFa/MP04/blob/main/uf3/compartir_impresora_linux.md)
  - [Còpies de seguretat programades amb NFS.](https://github.com/XaSaFa/MP04/blob/main/uf3/activitat_backup_nfs.md)
  

### Permisos a Linux
- [Permisos a Linux](https://github.com/XaSaFa/MP04/blob/main/uf3/permisos_linux.md)
- [umask](https://github.com/XaSaFa/MP04/blob/main/uf3/umask.md)
  
## Activitats

1. [Permisos Linux](activitat_permisos_linux.md)
2. [Net Use](https://github.com/XaSaFa/MP04/blob/main/uf3/activitat2.md)
3. [Carpetes personals](activitat_carpetes_personals.md)
4. [Compartir impressora](activitat_impressora.md)
5. [Polítiques de grup](activitat_directives_grup.md)
  
