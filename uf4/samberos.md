# Instal·lar Samba

```
sudo apt install samba
```

# Afegir usuari local a Samba

```
sudo smbpasswd -a xavi
```

# Directoris Home

Editem /etc/samba/smb.conf

```
sudo nano /etc/samba/smb.conf
```

Afegim al final.

```
[homes]
   comment = Home Directories
   browseable = yes
   read only = no
   create mask = 0700
   directory mask = 0700
   valid users = %S
```

Usuaris anònims:

```
sudo mkdir /var/samba
sudo chmod 777 /var/samba/
```

I a smb.conf

```
[public]
  comment = public anonymous access
  path = /var/samba/
  browsable =yes
  create mask = 0660
  directory mask = 0771
  writable = yes
  guest ok = yes
```

Reiniciem samba

```
sudo service smbd restart
```

Creo un parell de fitxers

```
touch /var/samba/fitxer-public 
touch /home/xavi/fitxer-home 
```
