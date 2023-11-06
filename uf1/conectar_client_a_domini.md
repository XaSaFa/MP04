# Connectar un client al domini

## Interfícies de Xarxa:

Per a connectar un client a domini necessitarem:

- Un ordinador client (farem servir una MV amb W10).
  - Aquest equip tindrà dos interfícies de xarxa: NAT i Xarxa interna.
- Un ordinador servidor (farem servir una MV amb W2016 server).
  - Aquest equip tindrà dos interfícies de xarxa: NAT i Xarxa interna.

Comprovem que tenim IP vàlida a l'ordinador client:

![image](https://github.com/XaSaFa/MP04/assets/110727546/f8d363b9-a18b-472c-853a-8b0674d7a1ba)

Comprovem que tenim IP vàlida a l'ordinador servidor:

![image](https://github.com/XaSaFa/MP04/assets/110727546/05a17753-fb08-43d4-902f-7dcce3804fbf)

Si mirem de fer ping entre les MV potser fallarà per culpa del Firewall del SO. Si el parèssim haurien de poder fer ping entre elles.

## Crear un usuari a Windows Server:

Crearem un usuari a Windows server per provar que funciona tot correctament.

![image](https://github.com/XaSaFa/MP04/assets/110727546/4951d2a9-aee7-41cd-99fc-1a3fe1261e14)

![image](https://github.com/XaSaFa/MP04/assets/110727546/0c05fb11-3983-4a47-bfb2-1c44a789eaf5)

## Canviar el DNS al client:

A la MV client canviarem la configuració de xarxa.

Seleccionem la interfície de xarxa d'adaptador intern i canviarem els paràmetres de IPv4.

![image](https://github.com/XaSaFa/MP04/assets/110727546/5bbbcbb4-9589-4db9-84d2-ffc220d36443)

Al camp DNS fiquem la IP de la MV del servidor.

![image](https://github.com/XaSaFa/MP04/assets/110727546/a9bf11dd-c3aa-45d6-b6b7-326cd4cab69d)

## Canviar el nom de domini:

![image](https://github.com/XaSaFa/MP04/assets/110727546/9b23f7a8-4f44-4b69-bb8a-c35d862f4520)

![image](https://github.com/XaSaFa/MP04/assets/110727546/0041a0c0-3c59-452e-af34-7345d5cbef74)

![image](https://github.com/XaSaFa/MP04/assets/110727546/2ace3668-0920-4b13-b902-ed96d16d27f5)

Ara Windows ens demanarà un usuari del domini:

![image](https://github.com/XaSaFa/MP04/assets/110727546/f3b83f54-07ea-4b40-a460-25cbf880ade8)



