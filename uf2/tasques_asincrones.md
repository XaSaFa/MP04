# Tasques asíncrones a Linux

Hi ha vegades que volem executar una tasca però l'ordinador que l'ha de fer està apagat, per aquest motiu no ens serveix programar la tasca amb cron.

En aquests casos podem utilitzar la comanda **anacron** (anachronistic cron).

## Instal·lar anacron

Comprovem si tenim instal·lat anacron al sistema, amb la comanda anacron, si no es així instal·lem anacron i reiniciem el sistema:

```
sudo apt install anacron
sudo reboot
```

## El fitxer /etc/anacrontab

Aquest fitxer serveix per escriure les tasques que volem realitzar.

![image](https://github.com/XaSaFa/MP04/assets/110727546/99cd516a-a592-4114-bf8f-d6d3fb5d2646)

Al fitxer tenim la següent informació:

- shell: Interpret de comandes per executar les tasques.
- home: La ruta del directori predeterminat.
- logname: El nom del compte d'usuari que executarà les tasques.

Cada tasca ocupa una línia amb la següent informació:

- Període d'execució: 1 vol dir cada dia (@daily), 7 vol dir cada setmana (@weekly), 30 vol dir cada mes (@monthly), si volem que s'executi cada 10 dies escrivim un 10.
- Retard d'execució: És un número que indica els minuts que espera anacron entre que detecta que ha d'executar una comanda i l'executa de veritat. Serveix per no col·lapsar el sistema només arrencar l'ordinador.
- Identificador: Nom que serveix per identificar la tasca. Serveix per si busquem informació als logs.
- Comanda: Instrucció que s'executarà.

**Exemple:**

Anem a crear una tasca que s'executi cada dia, amb un retard de 0 minuts i que es dirà backup_home_xavi.

Aquesta tasca executarà un script que guardarà els fitxers de la carpeta /home/xavi/Descargas a la carpeta /home/xavi/backup

A anacrontab afegirem la línia següent:

![image](https://github.com/XaSaFa/MP04/assets/110727546/48eb592a-5db7-459b-a61c-4baaf5026599)

I crearem el fitxer **SCRIPT** al que cridarem a /home/xavi/backup.sh

Aquest fitxer contindrà el següent:

![image](https://github.com/XaSaFa/MP04/assets/110727546/d093d860-8b74-425f-ad13-66259e59a429)

## Forçar execució d'Anacron

Per comprovar que funciona forcem l'execució d'anacron amb la comanda...

```
sudo anacron -f
```

I comprovem que s'ha executat.

**Exemple 2:**

Ara farem un script que copiï un fitxer anomenat prova.txt a un fitxer anomenat prova.txt seguit de la data i hora de quan es faci la còpia.

Per això crearem el fitxer prova.sh:

![image](https://github.com/XaSaFa/MP04/assets/110727546/6b0afd73-5520-45d1-a801-b7409f1451cb)

I després el modifiquem per ser executat per root:

```
chmod 700 prova.sh
```

Provem que funciona l'script:

```
sudo ./prova.sh
```

![image](https://github.com/XaSaFa/MP04/assets/110727546/d6fb0bfe-8868-4ec0-bd1e-62afc7069039)

Ara col·loquem la instrucció a anacron, farem que s'executi 1 vegada cada 3 dies, amb un retard de 2 minuts.

![image](https://github.com/XaSaFa/MP04/assets/110727546/84597a02-6fb5-4698-90cc-36430dd36d14)

Si forcem l'execució trigarà dos minuts en executar-se.

## Marques de temps

Al fitxer /var/spool/anacron es crearan fitxers per cada línia del fitxer anacrontab. 

![image](https://github.com/XaSaFa/MP04/assets/110727546/f668a048-a881-4f90-a73b-c14c5d64f6ac)

Aquests fitxers contenen la marca de temps de quan es va executar la tasca per última vegada.

![image](https://github.com/XaSaFa/MP04/assets/110727546/295b789e-8d68-4b9a-855d-d54fd4c51a49)

D'aquesta manera es controla quan s'ha de tornar a executar.



