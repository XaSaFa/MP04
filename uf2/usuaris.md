# Usuaris a Linux

## Superusuaris (root)

![image](https://github.com/XaSaFa/MP04/assets/110727546/a768d4ca-2a09-4d59-935a-1d8c94aa3be4)

A Linux els usuaris que tenen el control total sobre el sistema operatiu (instal·lar aplicacions, crear i esborrar carpetes i directoris a qualsevol punt de muntatge, crear usuaris, ...) es diuen **root** o **superusuaris**.

A Ubuntu l'usuari root per defecte està desactivat.

### sudo

La forma de fer que el sistema operatiu utilitzi els permisos de root a l'hora d'executar una comanda és afegint la paraula **sudo** davant de la instrucció, per exemple per instal·lar el servidor apache escriurem:

```
sudo apt install apache2
```

Llavors el sistema demanarà la contrasenya de root, la qual haurem d'escriure per poder executar la instrucció.

Quan fem servir la comanda sudo **el sistema estarà sense demanar la contrasenya de root durant 15 minuts**, per evitar que estiguem escrivint la contrasenya continuament.

### sudo su

Una altra forma d'executar comandes restringides al superusuari és transformar el nostre usuari a root, això s'aconsegueix amb la instrucció sudo su

![image](https://github.com/XaSaFa/MP04/assets/110727546/7df6b037-b79e-4f8e-a219-900fb1cf9266)

D'aquesta manera l'usuari serà root, però haurem de sortir de root quan volguem tornar a ser un usuari normal amb la comanda **exit**.

![image](https://github.com/XaSaFa/MP04/assets/110727546/391385c2-89a4-48ec-a96e-804e6e02c1bb)

