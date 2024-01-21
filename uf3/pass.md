# Passos

# 1.- Servidor IP fixa

Establim IP fixa amb netplan a la màquina servidor.

![image](https://github.com/XaSaFa/MP04/assets/110727546/4ac4efb9-2f0e-4736-91cb-d79c4cea9651)

Apliquem els canvis amb: 

```
sudo netplan apply
```

I comprovem que tenim la IP escollida:

![image](https://github.com/XaSaFa/MP04/assets/110727546/0fb4e3d3-7ba0-4cd2-918b-e8d2f11d397f)

# 2.- Nom del servidor

Primer canviem el nom de la màquina:

```
sudo hostnamectl set-hostname ldapserver.iaballester.cat
```

Després afegim a /etc/hosts les modificacions necessàries:

```
sudo nano /etc/hosts
```

![image](https://github.com/XaSaFa/MP04/assets/110727546/6bd18a5c-a168-42e0-ad9b-2c60585d205b)

# 3.- Actualitzem software

Actualitzarem els repositoris de software de l'equip amb la comanda següent:

```
sudo apt update
```

# 4.- Instal·la slapd i ldap-utils

Instal·lem el software necessari amb la comanda:

```
sudo apt install slapd ldap-utils
```

Ens demanarà la contrasenya d'administrador:

![image](https://github.com/XaSaFa/MP04/assets/110727546/43c0e5f4-29ef-4e99-9dc8-904cf3da978f)








