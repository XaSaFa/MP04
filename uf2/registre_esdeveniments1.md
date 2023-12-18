# Registre d'esdeveniments

A Linux tots els processos que registren informació ho fan al directori **/var/log** en forma de fitxers.

Aquests fitxers contenen informació amb el següent format:

- Data del succés.
- Hora.
- Nom de l'equip on s'ha produït.
- Programa o servei que ha originat el succés.
- Opcionalment pot aparèixer el PID del procés.
- Missatge infotmatiu que descriu el succés.

Els fitxers normalment són molt extensos, així que pot ser interessant buscar només els últims (amb tail) o específicament els que volem (amb cat i grep).

Exemple:

Si només volem veure les últimes 10 línies d'un fitxer utilitzem ```tail -f nomFitxer```.

Si només volem buscar línies amb un text determinat utilitzem ```cat nomFitxer | grep textABuscar```.

## Veure els registres per terminal



## Veure els registres en entorn gràfic

Podem veure els registres del sistema des de l'entorn gràfic, l'aplicació es diu "registres".

![image](https://github.com/XaSaFa/MP04/assets/110727546/e09e1ac1-9794-4d7f-aa92-42819d367790)

Es poden veure els registres de diferents apartats:

![image](https://github.com/XaSaFa/MP04/assets/110727546/a2f3cfe1-2ce5-45b3-a3dd-8c43cdf96231)

Per exemple a seguretat veurem els inicis de sessió.

![image](https://github.com/XaSaFa/MP04/assets/110727546/41322e7a-ca4b-4f62-8d17-03eb0eb9578a)

Fem un status del servei ssh i queda registrat a Aplicacions...

![image](https://github.com/XaSaFa/MP04/assets/110727546/c053d84e-88c1-49bd-bf21-8b90ebfdc32c)

Dins de registres podem cercar per mots.

![image](https://github.com/XaSaFa/MP04/assets/110727546/b3cf0f20-5386-4b33-b351-7357b54c5e6e)

També podem exportar els registres a un fitxer de text:

![image](https://github.com/XaSaFa/MP04/assets/110727546/f950edf3-3c20-4ec8-ade9-ab6a21972410)


