# Configurar client LDAP

Per a configurar un equip client i que es pugui autenticar mitjançant LDAP seguirem els següents passos:

## 1.- Actualitzar els repositoris

```
sudo apt update
```

## 2.- Instal·lar software

Instal·lem els paquests necessaris:

```
sudo apt install libnss-ldap libpam-ldap ldap-utils
```

Substituïm ldapi:/// per ldap:// i afegim la IP del servidor que hem configurat abans.

![image](https://github.com/XaSaFa/MP04/assets/110727546/137a71ee-1c49-4cc0-92f5-e2ba821d25c8)

Afegim el domini de LDAP:

![image](https://github.com/XaSaFa/MP04/assets/110727546/05237816-0cba-44f4-8bed-5d33f14a84ed)

Escollim la versió de LDAP (3):

![image](https://github.com/XaSaFa/MP04/assets/110727546/b6417d30-2938-4fff-b0ac-158447faadf1)

Escollim SI:

![image](https://github.com/XaSaFa/MP04/assets/110727546/dac39de2-a796-49c6-8eb3-6136cc93bfb7)

Després escollim NO:

![image](https://github.com/XaSaFa/MP04/assets/110727546/0cfe0a26-b2bc-470b-b85b-ba298cb0fefe)

Introduïm el compte administrador que vam crear al configurar el servidor:

![image](https://github.com/XaSaFa/MP04/assets/110727546/8a336709-bd13-4c0a-b604-eceacaaeae02)

I la contrasenya:

![image](https://github.com/XaSaFa/MP04/assets/110727546/e09eaa03-1a42-4a31-bda8-630a697184de)

A continuació seguirà la instal·lació.

![image](https://github.com/XaSaFa/MP04/assets/110727546/b848cb76-d63b-40ef-b50d-1fa7a6b0fc7f)

## Si ens equivoquem al configurar:

Executem la següent comanda i tornem a configurar.

```
sudo dpkg-reconfigure ldap-auth-config
```
