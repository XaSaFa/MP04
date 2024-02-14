# Connectar una unitat de xarxa

## net use

Hi ha diferents formes de connectar una unitat de xarxa, una d'elles és mitjançant la comanda net use.

Per fer servir net use necessitem un terminal de CMD de Windows.

Partim de la base de que tenim una carpeta compartida anomenada **public** al servidor anomenat **WIN-DPMGFEH4FMF**.

![image](https://github.com/XaSaFa/MP04/assets/110727546/c603ea50-b6da-4281-b1d7-e956f455ce53)

La comanda net use té els següents paràmetres:

net use <lletra unitat> <\\nom servidor\nom recurs compartit> </usuari>

## Connectar a una unitat de xarxa una vegada:

Podem connectar a un recurs compartit així:

```
net use f: \\WIN-DPMGFEH4FMF\public
```

![image](https://github.com/XaSaFa/MP04/assets/110727546/d6a22411-e966-45c4-a80d-6c48d6556316)

Una vegada es reinicii l'ordinador és desconnectarà la unitat.
