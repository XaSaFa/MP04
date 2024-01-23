# Autenticar clients a Linux

Hi ha diferents formes d'autenticar clients a nivell de xarxa al SO Linux, una d'elles és utilitzant PAM, NSS i LDAP.

La idea és utilitzar un servidor d'autenticació, de manera que cada vegada que un client s'hagi d'identificar ho faci a través del servidor.

Així aconseguim que el compte d'usuari no sigui local d'un equip si no que l'**usuari pugui identificar-se des de qualsevol equip configurat de la xarxa**.

![image](https://github.com/XaSaFa/MP04/assets/110727546/421e8253-d996-4cad-be15-e1710c62ff40)

Gracies a aquest servei obtindrem funcionalitats similars a les de Active Directory a Windows.

## NSS (Name Service Switch)

NSS és un servei que permet la resolució de noms d'usuari i contrasenyes (també de grups) mitjançant accés a diferents fonts d'informació. 

Originalment va ser escrit per Sun Microsystems i utilitzat al seu sistema operatiu Solaris.

Normalment, és a dir, a **nivell local**, aquesta informació es troba a:

/etc/passwd
/etc/shadow
/etc/group

Amb NSS es poden fer servir altres fonts per trobar la informació de grups i usuaris com LDAP.

D'aquesta manera es gestiona la informació dels usuaris sense utilitzar només una font local.

## PAM (Pluggable Authentication Modules)

Estableix una interfície entre els programes que demanen autenticació d'usuari i els mitjans d'autenticació, de forma que l'autenticació és transparent per als programes.

PAM va originar-se també a Sun Microsystems però es va implementar per primera vegada a Linux Red Hat com una eina de software lliure.

PAM es fa servir per canviar la forma d'autenticar-se dels programes sense canviar el sistema operatiu.

## LDAP (Lightweight Directory Access Protocol)

Es tracta d'un protocol que permet l'accés a un servei de directori sobre un entorn de xarxa.

Va ser creat originàriament a la Universitat de Michigan i publicat l'any 1993.

La versió 3 LDAPv3 va ser publicada l'any 1997.

OpenLDAP és una implementació de codi obert del protocol LDAP.

