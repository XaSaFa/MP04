# 1 Crea una nova unitat organitzativa anomenada clients.

![image](https://github.com/XaSaFa/MP04/assets/110727546/e817cba3-e9bc-4ffb-af34-4af519c7c4ae)

![image](https://github.com/XaSaFa/MP04/assets/110727546/a148178e-ea0e-4328-8e37-a11f5bc75c97)

```
dn: ou=clients,dc=dungeonofbits,dc=com
objectClass: top
objectClass: organizationalUnit
ou: clients 
```

# 2 Crea un grup anomenat catalunya.

![image](https://github.com/XaSaFa/MP04/assets/110727546/9ab90213-1502-4ce3-a28d-845db07985c3)

![image](https://github.com/XaSaFa/MP04/assets/110727546/b290913a-27e9-48d2-b193-8c1b2eb4bc6c)

```
dn: cn=catalunya,ou=clients,dc=dungeonofbits,dc=com
objectClass: top
objectClass: posixGroup
gidNumber: 10003
cn: clients
```

# 3 Dona d'alta els usuaris de la secció següent al grup catalunya de la uo clients.

![image](https://github.com/XaSaFa/MP04/assets/110727546/0f37f046-e5d6-4833-82be-181a2d1fb8c6)

![image](https://github.com/XaSaFa/MP04/assets/110727546/da09dba7-22ea-44de-ad7f-dfaffd82af73)

```
dn: uid=jmoyer,ou=clients,dc=dungeonofbits,dc=com
objectClass: top
objectClass: posixAccount
objectClass: inetOrgPerson
objectClass: person
uidNumber: 2005
gidNumber: 10003
ou: clients
cn: Joseph
uid: jmoyer
givenName: Joseph
sn: Moyer
homeDirectory: /home/jmoyer
loginShell: /bin/bash
userPassword: {SSHA}+qRgNVXlKk4CCuRh8cT85i2I1VdG5aHk
mail: teresa51@gmail.com
telephoneNumber: 628614179
postalAddress: 06875 Hannah Square
postalCode: 25001
l: Lleida
```

```
ldapsearch -xLLL -b "dc=dungeonofbits,dc=com" "(&(givenName=xavi)(sn=*cho*))"
```
