# Activitats de backups i programació de tasques

Nota: X és el teu cognom.

1. dump i restore
- Crea una carpeta al teu home anomenada /Xbackup.
- Dins la carpeta guarda dues imatges.
- Fes un backup amb dump al fitxer /tmp/Xbackup de la carpeta.
- Esborra les imatges.
- Recupera amb restore les imatges a la carpeta que ara està buida.

2. tar
- Repeteix l'activitat anterior amb tar.

3. rsync
- Repeteix l'activitat anterior amb tar.

4. cron
- Fes una tasca que reiniciarà l'ordinador en un parell de minuts i comprova que funciona.

4. cron
- Fes un script que:
  - guardi la data i hora de l'ordinador i la guardi al fitxer control.txt
  - guardi l'estat d'ocupació dels discos de l'ordinador.
  - La informació es guarda al fitxer de forma acumulativa, és a dir, no s'esborra la informació anterior.
- Fes una tasca que executi l'script cada minut.

PISTA: Podeu utilitzar les comandes "df" i "date" a més de l'operador ">>".

EXEMPLE RESULTAT FITXER:

![image](https://github.com/XaSaFa/MP04/assets/110727546/063d26df-99c0-48f8-87f6-ee61eb78e2a8)


