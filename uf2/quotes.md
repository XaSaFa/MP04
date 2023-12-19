# Quotes de disc

![image](https://github.com/XaSaFa/MP04/assets/110727546/5603e8d2-5a76-44f7-a315-802cdba4ddb4)

Les quotes de disc serveixen per limitar l'espai que pot utilitzar un usuari del sistema.

Existeixen diferents tipus de limitacions:

- Podem limitar l'espai de blocs de disc, d'aquesta manera limitem l'espai màxim que es pot ocupar.
- Podem limitar els i-nodes, és a dir, el nombre d'objectes d'emmagatzematge (fitxers o directoris).

A més les limitacions poden ser rígides o flexibles:

- Les rígides (o hard) fan que el sistema operatiu impideixi que el límit es sobrepassi.
- Les flexibles (soft) fan que el sistema operatiu avisi quan es sobrepassin els límits.

## Instal·lar el servei de quotes

Instal·larem el servei de quotes orientat a limitra l'ús de disc al directori **home** dels usuaris.

Comencem per instal·lar els paquets per a gestionar quotes a Linux:

```
sudo apt install quota quotatool
```

![image](https://github.com/XaSaFa/MP04/assets/110727546/7ecfcd08-eea2-48c4-bac5-5d8c97272b53)

Després hem d'indicar que utilitzarem quotes al directori /home editant el fitxer **/etc/fstab**

El canviarem de:

![image](https://github.com/XaSaFa/MP04/assets/110727546/fe054819-12f6-4106-af4b-d9e7c673f630)

a: 

![image](https://github.com/XaSaFa/MP04/assets/110727546/544d9a3d-3070-4498-8705-2b2679b137d0)

on usrquota indica que utilitzarem quota d'usuari i grpquota quota de grup.

Després remontem el sistema de fitxers de /home amb la comanda:

```
sudo mount -o remount,rw /home
```

