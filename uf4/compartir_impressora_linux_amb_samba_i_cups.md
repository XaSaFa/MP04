# Compartir una impressora de Linux amb Samba i CUPS.

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
sudo service smdb restart
sudo service cups restart
```

# Pas 5.- Obrim CUPS a Windows

Anem a una MV amb Windows que estigui a la mateixa xarxa que la MV Linux i obrim un navegador.

A la barra d'adreces escrivim la ip de la MV Linux seguida de ":" i el número de port, que és 631.

![image](https://github.com/XaSaFa/MP04/assets/110727546/47967496-77cc-4a20-9bca-3e3108740765)


