# Programar tasques a Linux

![image](https://github.com/XaSaFa/MP04/assets/110727546/ff8ddfe4-f2ff-4050-8175-8398974e963c)

A Linux normalment s'utilitza el programa **cron** per programar tasques, aquest programa consta del dimoni crond i uns fitxers de configuració.

En principi cron s'inicialitza amb el sistema operatiu i s'activa cada minut per comprovar si hi ha tasques per executar.

## Crear una tasca

Per a crear una tasca utilitzarem la comanda crontab amb l'argument -e.

```
crontab -e
```

La primera vegada que el fem servir ens farà escollir un editor de textos:

![image](https://github.com/XaSaFa/MP04/assets/110727546/00d018b7-161e-4185-848d-5bbe530efcf3)

En aquest cas jo faré servir nano i em sortirà aquest fitxer de text:

![image](https://github.com/XaSaFa/MP04/assets/110727546/0ee5329e-09ec-49de-901d-131780e738f1)

Les següents vegades que fem servir la comanda farà servir el mateix editor de text, si alguna vegada volem canviar l'editor podem utilitzar la comanda:

```
sudo update-alternatives --config editor
```

El fitxer de text ens permet introduïr línies amb les tasques que volem programar, **CADA LÍNIA ÉS UNA TASCA**.

Les línies es composen de sis dades:

1. Minut: entre 0 i 59.
2. Hora: entre 0 i 23.
3. Dia del mes: Entre 1 i 31.
4. Mes de l'any: Entre 1 i 12.
5. Dia de la setmana: Pot escriure's de dues formes:
  - Valor entre 0 i 7: 0 i 7 = diumenge, 1 = dilluns, 2 = dimarts...
  - Valors en text: sun, mon, tue, wed, thu, fri i sat.    
6. Ordre a executar-se al shell: Qualsevol cosa entre el dia de la setmana i el final de la línia s'envia a la shell, si hi ha un símbol de percentatge % es talla la línia, així que si hem d'enviar un símbol de percentatge haurem d'escriure'l amb un caràcter de barra inversa davant (\%).

Els primers 5 valors es poden expressar com:

- Valors individuals: Per exemple minut 5 -> 5.
- Rang de valors: Per exemple minuts 5 a 10 -> 5-10.
- Llista de valors: Separats per comes, per exemple minuts 1,3 i 5: -> 1,3,5.
- Tots els valors possibles: Un asterisc -> *.

Exemple: Programem l'apagat diari de l'ordinador a les 20:15.

| Minut | Hora | Dia del mes | Mes | Dia de setmana | Ordre |
|----------|----------|----------|----------|----------|----------|
| 15    | 20   | *   | *    | *   | /sbin/poweroff   |

![image](https://github.com/XaSaFa/MP04/assets/110727546/e158755f-c9ef-486a-b5c1-cbf2f87c13fe)




