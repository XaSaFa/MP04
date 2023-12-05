# Activitat 1 - Gestió de disc a Linux

Per a fer les activitats següents mostra a cada sortida el prompt on es veu que la màquina es diu **MP-04-X** (on X és el teu cognom).

1. Canvia el nom de l'equip tant amb hostnamectl com a /etc/hosts.

![image](https://github.com/XaSaFa/MP04/assets/110727546/b291769b-7568-4fc7-9343-b02d2af21057)

2. Mira si hi ha una versió LTS nova de Linux

![image](https://github.com/XaSaFa/MP04/assets/110727546/ae4b36bc-b746-4c84-8e14-2df686b2358f)

3. Utilitza la comanda df i mostra la sortida amb lectura per a humans.

![image](https://github.com/XaSaFa/MP04/assets/110727546/b032c64d-780f-46f5-94b4-021f34e8f765)

4. Personalitza la comanda df per que mostri a la sortida tota la informació normal i també el tipus de sistema de fitxers.

![image](https://github.com/XaSaFa/MP04/assets/110727546/855ce0b2-a75f-44a8-956d-7ab1cf606d93)

5. Personalitza la comanda df fent que les dades que es mostrin siguin, origen de dades, espai disponible i sistema de fitxers, només per als que utilitzin ext4 (fes servir grep).

![image](https://github.com/XaSaFa/MP04/assets/110727546/7b7e3fc8-c85f-4c78-ab11-58bd004b740b)

6. Afegeix, si no ho has fet, un segon disc dur virtual de 1GB a la MV.

![image](https://github.com/XaSaFa/MP04/assets/110727546/5a7236fa-5971-4b46-8e4a-ba5ba51140ba)

7. Fent servir fdisk mostra el tamany del segon disc.

![image](https://github.com/XaSaFa/MP04/assets/110727546/755d2c16-2c1b-47c5-a23b-b73cd6826576)

8. Crea una nova partició primària de 256MB al segon disc.

![image](https://github.com/XaSaFa/MP04/assets/110727546/a21d2819-5714-4b66-b088-95053cfe1d03)

9. Mostra la nova partició creada amb fdisk.

![image](https://github.com/XaSaFa/MP04/assets/110727546/49ccfc1e-1de2-40c1-bc60-6c9efb4dd135)

10. Mostra l'espai lliure del disc amb fdisk.

![image](https://github.com/XaSaFa/MP04/assets/110727546/ca768670-3a89-40f2-b51b-8fe31fe3e211)
    
11. Esborra la partició amb fdisk.

![image](https://github.com/XaSaFa/MP04/assets/110727546/99115004-b566-4d36-880c-978479ae976d)

12. Crea les següents particions al segon disc.
  - Primària 100MB.
  - Primària 400MB.
  - Estesa de tot el tamany restant (uns 500MB).
  - Lògica de 250MB.
  - Lògica de la resta del tamany de disc.
13. Mostra les particions creades i escriu-les amb la comanda w.

![image](https://github.com/XaSaFa/MP04/assets/110727546/9bf1443b-03ca-491c-a125-9dc36fe56081)

![image](https://github.com/XaSaFa/MP04/assets/110727546/c2f168d2-2d73-4680-9319-6d8d3ade9123)

14. Formateja les particions primàries com ext4.

![image](https://github.com/XaSaFa/MP04/assets/110727546/fc691047-e8c4-42f8-b03c-e8bbf69e163b)

15. Formateja les particions esteses com NTFS.

![image](https://github.com/XaSaFa/MP04/assets/110727546/39937633-fb40-4f50-9436-4c6115f00a54)

16. Munta les particions a les carpetes següents:
  - /dev/sda1 a /disc1-X (on X és el teu cognom)
  - /dev/sda2 a /disc2-X (on X és el teu cognom)
  - /dev/sda5 a /disc3-X (on X és el teu cognom)
  - /dev/sda6 a /disc4-X (on X és el teu cognom)
![image](https://github.com/XaSaFa/MP04/assets/110727546/c2823125-2ea7-4133-ac4a-99a7f532ed78)
![image](https://github.com/XaSaFa/MP04/assets/110727546/4e5a2121-124d-482d-b187-82749b2eac94)
![image](https://github.com/XaSaFa/MP04/assets/110727546/053d8b6f-57df-4e84-ab3a-9e837663b9a1)
17. Prova que pots accedir als discos (accedeix i utilitza la comanda pwd).
 
    ![image](https://github.com/XaSaFa/MP04/assets/110727546/3963a4da-f4a9-4c3b-a490-878f61e868fb)

18. Mostra les particions i punt de muntatge amb la comanda lsblk

![image](https://github.com/XaSaFa/MP04/assets/110727546/0ffa9db6-de63-4cbf-bb78-98694e1c7a33)

