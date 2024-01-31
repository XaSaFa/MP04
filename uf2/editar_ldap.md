En aquest apartat veurem com consultar, editar i esborrar elements del directori.

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

Si volem fer una consulta amb més d'una condició utilitzem un AND representat pel símbol "&", al següent exemple mostrem l'usuari que té givenname xavi i el seu cognom conté "cho".

```
ldapsearch -xLLL -b "dc=dungeonofbits,dc=com" "(&(givenName=xavi)(sn=*cho*))"
```

![image](https://github.com/XaSaFa/MP04/assets/110727546/2655e559-75f7-4f2d-8268-08babd7ff659)

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

En aquest altre exemple modifiquem el cognom de Sancho a Molina:

![image](https://github.com/XaSaFa/MP04/assets/110727546/2cdcd0da-22b5-4597-97d7-1ef1cf0a9f15)

![image](https://github.com/XaSaFa/MP04/assets/110727546/af631869-1b94-482a-abdb-c71b013a8610)

# Eliminar elements del directori

Per a eliminar elements utilitzem la comanda **ldapdelete**.

Per exemple anem a eliminar un usuari anomenat kerrigan, amb uid=kerrigan:

![image](https://github.com/XaSaFa/MP04/assets/110727546/3de7a890-fc4d-4eeb-868d-5ad0760c73cd)

Per esborrar el grup grupoDOS fem:

![image](https://github.com/XaSaFa/MP04/assets/110727546/9c739c02-f6a7-43dc-bc4c-e89dd0b2e803)


