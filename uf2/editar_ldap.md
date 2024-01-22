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


