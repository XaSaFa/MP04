```
sudo apt update
```

```
sudo apt install samba smbclient winbind
```

```
wget https://download.microsoft.com/download/c/3/c/c3cd85c0-0785-4cf7-a48e-cdc9b8e20108/Administrative%20Templates%20\(.admx\)%20for%20Windows%2010%20October%202022%20Update.msi
```

![image](https://github.com/user-attachments/assets/d1630a4a-70f1-4196-9e0e-4bd71813f285)


```
sudo apt install msitools
```
```
sudo hostnamectl set-hostname AKIRA
```

Editar el fitxer /etc/hosts 

![image](https://github.com/user-attachments/assets/7947bc23-05f8-4c86-8e96-831b41a601ad)

Instal·lem el servei kerberos

```
sudo apt install krb5.config
```

El nostre domini serà NEOTOKYO.LOCAL.

![image](https://github.com/user-attachments/assets/277f41d2-084c-409c-be56-b56b076cace8)

![image](https://github.com/user-attachments/assets/49fafac7-9c7f-4e73-ac83-e8a4fbe5d0ef)

![image](https://github.com/user-attachments/assets/ce6d8abc-6b01-41f6-b2e1-13d48df1c30e)

```
sudo mv /etc/samba/smb.conf /etc/samba/smb.conf.OLD
```

```
sudo samba-tool domain provision
```

![image](https://github.com/user-attachments/assets/8f5bbab9-fa39-4b8a-b475-c64977c02635)

```
sudo cp /var/lib/samba/private/krb5.conf /etc/
```

```
sudo systemctl stop smbd nmbd winbind systemd-resolved
sudo systemctl disable smbd nmbd winbind systemd-resolved
```

```
sudo systemctl unmask samba-ad-dc
```

```
sudo mv /etc/resolv.conf /etc/resolv.conf.OLD
```

```
sudo nano /etc/resolv.conf
```

![image](https://github.com/user-attachments/assets/8208a7d6-1ad6-4f91-a108-f4d8b8187a83)

```
sudo systemctl start samba-ad-dc
sudo systemctl enable samba-ad-dc
```

```
sudo samba-tool domain level show
```

![image](https://github.com/user-attachments/assets/4c845bd1-119e-444b-a832-af0c3352b3b0)

```
sudo samba-tool user create kaneda
```

![image](https://github.com/user-attachments/assets/87a624e3-6dec-4c63-bcfd-09d7183a2a7c)

```
host -t SRV _ldap._tcp.NEOTOKYO.LOCAL
host -t SRV _kerberos._udp.NEOTOKYO.LOCAL
host -t A AKIRA.NEOTOKYO.LOCAL
```

![image](https://github.com/user-attachments/assets/e4808a8c-c2b1-4da2-b8e6-43ec0aa20f95)

```
sudo smbclient -L AKIRA.NEOTOKYO.LOCAL -U 'administrator'
```

![image](https://github.com/user-attachments/assets/d6e6c56f-e1db-442b-af54-abca69c9bd2f)

Editar el fitxer smb.conf

```
sudo nano /etc/samba/smb.conf
```

![image](https://github.com/user-attachments/assets/b5da1389-dbde-4631-9ddc-44fe286372e7)

```
sudo service samba-ad-dc restart
```

```
samba-tool gpo admxload -U Administrator
```

```
msiextract 
```

![image](https://github.com/user-attachments/assets/cdb5272e-6af6-4eaf-8a93-d7a640df213d)


```
samba-tool gpo admxload -U Administrator --admx-dir=/Program\ Files/Microsoft\ Group\ Policy/Windows\ 10\ October\ 2022\ Update\ \(22H2\)/PolicyDefinitions/
```

![image](https://github.com/user-attachments/assets/83f58b25-226b-4d12-9474-fd233931036a)


A Windows 10


![image](https://github.com/user-attachments/assets/e90880f0-7fee-48ce-b987-1235a74d5d19)


![image](https://github.com/user-attachments/assets/fa4177b4-6b5e-4588-ba0b-26ee57c0b0ca)

![image](https://github.com/user-attachments/assets/b0389192-446f-40fd-b3bd-d9b770e873df)

![image](https://github.com/user-attachments/assets/5c574c67-cff5-4224-9578-09b7613a3916)

![image](https://github.com/user-attachments/assets/8ae83990-ccd6-4cbd-b306-f94425484787)


