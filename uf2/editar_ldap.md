# Consultar elements al directori

Si volem buscar informació d'elements dins del directori tenim la comanda **ldapsearch** disponible.

Per exemple, per buscar el directory home i el uid de l'usuari xavi utilitzarem la comanda:

```
ldapsearch -xLLL -b "dc=dungeonofbits,dc=com" uid=xavi homeDirectory uid
```

![image](https://github.com/XaSaFa/MP04/assets/110727546/73ec80a9-7dee-4478-91df-f696d402e67c)

Amb els paràmetres:

- -x: Indica que utilitzem autenticació simple.
- -LLL: Serveix per que la sortida sigui del tipus LDAPv1.
- -b: Va seguit del punt de l'arbre on ha de començar la cerca.
- Després va la condició a cumplir pels objectes cercats. Podem utilitzar * com a comodí.
- Per últim posem el nom dels atributs que volem que es mostrin com a resultat.

# Modificar elements del directori

Per modificar elements dispossem de la comanda **ldapmodify**.

Per exemple anem a modificar el mail de l'usuari creat anteriorment xavi, per a fer-ho crearem un fitxer de text com aquest:

![image](https://github.com/XaSaFa/MP04/assets/110727546/2ab0709c-7219-4034-84e2-536a2fc3f6c3)

On fiquem l'identificador de l'usuari i les dades a modificar, en aquest cas el correu electrònic.

Abans del canvi el mail de l'usuari era així:

![image](https://github.com/XaSaFa/MP04/assets/110727546/b88515ff-8b8d-4e26-9424-c5064933cb9a)

Apliquem la comanda ldapmodify:

![image](https://github.com/XaSaFa/MP04/assets/110727546/b7dce1c1-b5e5-4fda-997a-94494f178182)

Després del canvi el mail de l'usuari és:

![image](https://github.com/XaSaFa/MP04/assets/110727546/c056c009-a004-4355-b146-19e4bbb1362d)

Com veiem hem modificat el mail de l'usuari però podem modificar la resta de camps també.


