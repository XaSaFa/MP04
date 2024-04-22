![image](https://github.com/XaSaFa/MP04/assets/110727546/febd6892-aa72-4ba2-aa34-8f7d6bb00ebb)# Compartir una impressora de Linux amb Samba i CUPS.

Necessitem tenir un equip Linux amb una impressora.

# Pas 1.- Instal·lar i configurar Samba.

Instal·lem samba.

```
sudo apt install samba
```

Modifiquem la configuració de samba.

```
sudo nano /etc/samba/smb.conf
```

Hem de deixar la part de impressores així:

![image](https://github.com/XaSaFa/MP04/assets/110727546/8802a3e2-70ef-4a69-ae39-4e85ccdced48)

# Pas 2.- Instal·lar CUPS.

```
sudo apt install cups 
```

# Pas 3.- Configurar CUPS.

Editem el fitxer de configuració de CUPS.

```
sudo nano /etc/cups/cupsd.conf
```

Hem de fer les següents modificacions:

![image](https://github.com/XaSaFa/MP04/assets/110727546/bf4af785-fb2d-4130-9dc4-a76cf1105c20)

![image](https://github.com/XaSaFa/MP04/assets/110727546/4f802831-9911-4ff9-b661-19c4ac5c8c80)

# Pas 4.- Reiniciem els serveis.

```
sudo service smbd restart
sudo service cups restart
```

# Pas 5.- Obrim CUPS a Windows

Anem a una MV amb Windows que estigui a la mateixa xarxa que la MV Linux i obrim un navegador.

A la barra d'adreces escrivim la ip de la MV Linux seguida de ":" i el número de port, que és 631.

![image](https://github.com/XaSaFa/MP04/assets/110727546/47967496-77cc-4a20-9bca-3e3108740765)

# Pas 6.- Afegir impressora a CUPS

![image](https://github.com/XaSaFa/MP04/assets/110727546/eb6625d7-ed3f-4af5-9d61-1f6890e825e0)

![image](https://github.com/XaSaFa/MP04/assets/110727546/3216947c-83b6-4196-adeb-79cd1344247a)

![image](https://github.com/XaSaFa/MP04/assets/110727546/9c4f4942-c59f-4ebe-b86d-e16f5dde4fcb)

![image](https://github.com/XaSaFa/MP04/assets/110727546/708bde0a-8237-4a0c-b90e-22de613eb3e3)

![image](https://github.com/XaSaFa/MP04/assets/110727546/3a1bb54b-2ee9-4b07-8a43-c8bc7251ee02)

![image](https://github.com/XaSaFa/MP04/assets/110727546/a71da6aa-fd4e-4f4f-89f0-79922c0b4a43)

![image](https://github.com/XaSaFa/MP04/assets/110727546/81caf35e-8310-408b-8d01-5f6e4715d04d)

![image](https://github.com/XaSaFa/MP04/assets/110727546/1b4c05e1-aa5d-471b-bf79-99a336e17039)

![image](https://github.com/XaSaFa/MP04/assets/110727546/d862ca6f-27c7-430f-8084-7cdfda8251af)

# Pas 7.- Afegir la impressora a Windows

Anem a la secció impressores de CUPS.

![image](https://github.com/XaSaFa/MP04/assets/110727546/8a4cdb4f-8957-4524-9ea6-d10d50f1aa91)

Seleccionem la impressora que volem utilitzar.

![image](https://github.com/XaSaFa/MP04/assets/110727546/c8487bea-5590-4bfe-a854-fb39da58b9cd)

I copiem l'adreça de la impressora de la barra d'adreces del navegador.

![image](https://github.com/XaSaFa/MP04/assets/110727546/acb7179b-1d99-468a-bacd-2a7bb1ba1d86)

Anem a Configuració de Windows-> Dispositius

![image](https://github.com/XaSaFa/MP04/assets/110727546/15e301c7-162d-4db4-897b-1b2e0d9c4cf4)

Anem a Impressores i escàners i cliquem a afegir.

![image](https://github.com/XaSaFa/MP04/assets/110727546/4395a1fd-5224-4d03-8a32-049d14955ed1)

![image](https://github.com/XaSaFa/MP04/assets/110727546/a974eed3-494d-494d-8622-369d1678db47)

![image](https://github.com/XaSaFa/MP04/assets/110727546/c0d8ea67-3cbe-4a6f-b74a-1be83e4aa182)

![image](https://github.com/XaSaFa/MP04/assets/110727546/bbbcfb66-5ebf-4e5e-9432-602e9aacd519)
![image](https://github.com/XaSaFa/MP04/assets/110727546/dd0d873a-c205-4a29-8c68-86ee68790994)

![image](https://github.com/XaSaFa/MP04/assets/110727546/0b4dba83-4100-4ae6-b52a-5291edd752c4)
![image](https://github.com/XaSaFa/MP04/assets/110727546/0d2e86b0-bc30-49fb-a7d0-824ad283dc56)
![image](https://github.com/XaSaFa/MP04/assets/110727546/7a446090-167d-4718-8590-fb1df80c63b9)
![image](https://github.com/XaSaFa/MP04/assets/110727546/fb479e74-d9d3-4500-a4ad-f32bfcf95f33)
![image](https://github.com/XaSaFa/MP04/assets/110727546/7d622d94-d4c8-4a8c-adc6-a712739c3d72)


