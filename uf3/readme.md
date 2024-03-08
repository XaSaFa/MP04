# UF3 - Compartició de recursos i seguretat

![image](https://github.com/XaSaFa/MP04/assets/110727546/1dcee92e-e0ca-46a9-9115-3c300955b547)

## Programació

- [Programació UF3](programacio.md)

## Permisos i drets

- [Permisos i drets](permisos_i_drets.md)

## Compartir recursos

### Windows

Per compartir recursos a Windows necessitem dues MV:
- Windows Server 2016 (teniu la OVA a Moodle).
- Windows 10 (teniu la OVA a Moodle).

- A Windows Server heu d'instal·lar active directory i crear un domini anomenat COGNOM.COM (aquí teniu enllaços a la teòria del tema 1):
  - [Instal·lar rol AD](https://github.com/XaSaFa/MP04/blob/main/uf1/instalar_domini.md).
  - [Promocionar el controlador de domini](https://github.com/XaSaFa/MP04/blob/main/uf1/instalar_domini2.md)
  - [Després heu d'unir el client al servidor](https://github.com/XaSaFa/MP04/blob/main/uf1/conectar_client_a_domini.md)

- Connectar unitats de xarxa i recursos de xarxa
  - [Net use](connectar_unitat_xarxa.md)
  - [Connectar a unitat de xarxa i recurs de xarxa de forma gràfica](connectar_unitat_xarxa_visual.md)
  - [Crear una carpeta personal per als usuaris del domini](carpeta_personal_windows.md)
  - [Compartir impressora](compartir_impressora.md)

- Directives de grup
  - [Crear una directiva de grup per una unitat organitzativa](directives.md)
 
### Linux

Per compartir recursos a Linux necessitem dues MV:
- Ubuntu 22.04LTS (Servidor).
- Linux Mint (client).

- NFS:
  - [Què és NFS](nfs0.md)
  - [Instal·lar NFS al server](nfs1.md)
  - [Instal·lar NFS al client](nfs2.md)
  - [Crear el recurs compartit](nfs3.md)
  - [Accedir a la carpeta compartida des d'un client](nfs4.md)
  - [Muntar automàticament les carpetes compartides](nfs5.md)
  - [Muntar la carpeta home del servidor per cada usuari client](nfs6.md)
  

### Permisos a Linux
- [Permisos a Linux](permisos_linux.md)
- [umask](umask.md)
  
## Activitats

- [Activitat 1 - Permisos Linux](activitat1.md)
- [Activitat 2 - net use](activitat2.md)
- [Activitat 3 - Crea una carpeta personal per als usuaris d'un domini seguint el tutorial](carpeta_personal_windows.md)
- [Activitat 4 - Comparteix impressora a Windows](activitat4.md)
- [Activitat 5 - Crear una directiva de grup](activitat5.md)
  
