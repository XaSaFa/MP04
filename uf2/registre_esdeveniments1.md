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

Si només volem buscar  fitxer utilitzem ```tail -f nomFitxer```.
