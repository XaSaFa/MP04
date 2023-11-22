## fdisk

fdisk (Format Disk) és una comanda que ens permet manipular particions dels nostres discs durs.

Podem fer servir fdisk per veure el tamany d'un.

![image](https://github.com/XaSaFa/MP04/assets/110727546/de394410-3102-4da2-ac7c-c28ea8296a12)

Per veure les particions d'un disk podem utilitzar la comanda fdisk -l nom de disc, per exemple:

![image](https://github.com/XaSaFa/MP04/assets/110727546/f6e2de5e-db3d-4223-9134-7c7783e4d6f5)

Per manipular un disc concret escrivim la comanda sudo fdisk nom de disc, per exemple:

![image](https://github.com/XaSaFa/MP04/assets/110727546/4aa52999-f590-4cbe-a3d7-5b2acea16dff)

Les comandes de fdisk apareixen al escriure m:

![image](https://github.com/XaSaFa/MP04/assets/110727546/64460ac3-99c6-49b4-be25-095fbe2d338e)

Per veure l'espai lliure escriurem F:

![image](https://github.com/XaSaFa/MP04/assets/110727546/31885fbb-2fa9-4060-aac1-d9d5348b23a1)

Aquí es veu que no hi ha espai lliure.

## Crear una nova partició

Utilitzem un disc buit que estarà muntat a /dev/sdb i per a la nova partició escrivim **n**.

![image](https://github.com/XaSaFa/MP04/assets/110727546/52b9d854-397f-4324-89a9-fa7b35185516)

## Mostrar particions

Amb **p** podem veure les particions creades:

![image](https://github.com/XaSaFa/MP04/assets/110727546/9c8ed257-ae67-4801-ad5e-f0afd5f1ca82)

## Canviar el sistema de fitxers d'una partició

Amb t podem canviar el sistema de fitxers d'una partició, a l'exemple canviem a FAT16

![image](https://github.com/XaSaFa/MP04/assets/110727546/3a900f3f-828e-4bf1-90f9-d090b54e9d64)

Quan ho fem podem llistar els sistemes de fitxers amb L:

![image](https://github.com/XaSaFa/MP04/assets/110727546/7bbb89ea-493e-43e4-a67e-201befb9f0ec)


