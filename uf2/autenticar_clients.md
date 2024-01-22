# Autenticar clients a Linux

Hi ha diferents formes d'autenticar clients a nivell de xarxa al SO Linux, una d'elles és utilitzant PAM, NSS i LDAP.

La idea és utilitzar un servidor d'autenticació, de manera que cada vegada que un client s'hagi d'identificar ho faci a través del servidor.

Així aconseguim que el compte d'usuari no sigui local d'un equip si no que l'**usuari pugui identificar-se des de qualsevol equip configurat de la xarxa**.

![image](https://github.com/XaSaFa/MP04/assets/110727546/421e8253-d996-4cad-be15-e1710c62ff40)

Gracies a aquest servei obtindrem funcionalitats similars a les de Active Directory a Windows.

