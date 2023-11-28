# Activitat 1 - Gestió de disc a Linux

Per a fer les activitats següents mostra a cada sortida el prompt on es veu que la màquina es diu **MP-04-X** (on X és el teu cognom).

1. Canvia el nom de l'equip tant amb hostnamectl com a /etc/hosts.
2. Mira si hi ha una versió LTS nova de Linux
3. Utilitza la comanda df i mostra la sortida amb lectura per a humans.
4. Personalitza la comanda df per que mostri a la sortida tota la informació normal i també el tipus de sistema de fitxers.
5. Personalitza la comanda df fent que les dades que es mostrin siguin, origen de dades, % d'espai disponible i sistema de fitxers, només per als que utilitzin ext4 (fes servir grep), com a l'exemple:
![image](https://github.com/XaSaFa/MP04/assets/110727546/092bbba6-e3d9-404c-890c-667f77a9a7a5)
6. Afegeix, si no ho has fet, un segon disc dur virtual de 1GB a la MV.
7. Fent servir fdisk mostra el tamany del segon disc.
8. Crea una nova partició primària de 256MB al segon disc.
9. Mostra la nova partició creada amb fdisk.
10. Mostra l'espai lliure del disc amb fdisk.
11. Esborra la partició amb fdisk.
12. Crea les següents particions al segon disc.
  - Primària 100MB.
  - Primària 400MB.
  - Estesa de tot el tamany restant (uns 500MB).
  - Lògica de 250MB.
  - Lògica de la resta del tamany de disc.
13. Mostra les particions creades i escriu-les amb la comanda w.
![image](https://github.com/XaSaFa/MP04/assets/110727546/c2f168d2-2d73-4680-9319-6d8d3ade9123)

14. Formateja les particions primàries com ext4.
15. Formateja les particions esteses com NTFS.
16. Munta les particions a les carpetes següents:
  - /dev/sda1 a /disc1-X (on X és el teu cognom)
  - /dev/sda2 a /disc2-X (on X és el teu cognom)
  - /dev/sda5 a /disc3-X (on X és el teu cognom)
  - /dev/sda6 a /disc4-X (on X és el teu cognom)
17. Prova que pots accedir als discos (accedeix i utilitza la comanda pwd).
18. Mostra les particions i punt de muntatge amb la comanda lsblk

