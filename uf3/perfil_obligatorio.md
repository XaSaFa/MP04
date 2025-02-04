# Crear un usuari amb perfil obligatori

## Pas 1 - Donar privilegi a l'usuari 

![image](https://github.com/user-attachments/assets/005779a7-e6f1-4f19-85a6-bd9f57e71aa0)

![image](https://github.com/user-attachments/assets/de12ee98-e2db-4ff4-9848-3958775701be)

![image](https://github.com/user-attachments/assets/fa4548c0-810e-466e-aa44-27f940abbe77)

Iniciem sessió al server com l'usuari anterior

![image](https://github.com/user-attachments/assets/27f64667-3d78-4cbb-a2d7-fe09f8775291)

Fem modificacions

![image](https://github.com/user-attachments/assets/d86dcea6-1bff-4c7d-a7f2-a270de550f0c)

Tanquem sessió i iniciem com Administrador

## Creem una carpeta compartida

Aquesta carpeta estarà a C: i es dirà "Perfiles"

![image](https://github.com/user-attachments/assets/e49710ed-38ae-4916-a106-898648e23915)

![image](https://github.com/user-attachments/assets/d24881f2-6f20-4027-bf54-619ed6f141b9)

La compartim amb els usuaris necessaris, en aquest cas podem utilitzar "Todos".

![image](https://github.com/user-attachments/assets/91027be9-694c-418c-8112-1b6db3c18947)

![image](https://github.com/user-attachments/assets/37bc87c7-a0ba-485d-8ef3-bcf2199de00f)

## Pas 2 - Modificar els fitxers al server

Accedim a C:

![image](https://github.com/user-attachments/assets/5f339438-e0c9-4f36-9126-f95e477298ff)

![image](https://github.com/user-attachments/assets/1de277a2-f686-401b-8786-d066afcb2522)

![image](https://github.com/user-attachments/assets/2d7b8c24-5b68-472e-8625-cce53cad119e)

Enganxem la carpeta a C:\Perfiles

![image](https://github.com/user-attachments/assets/9edeaccd-1e19-4fce-bf38-50f82eb723d2)

Canviem el nom de la carpeta afegint ".V5":

![image](https://github.com/user-attachments/assets/5a221cb7-2632-42bf-b702-585d7f2b71e1)

Dins la carpeta mostrem els fitxers ocults

![image](https://github.com/user-attachments/assets/f0f2f96c-aa16-4c8d-a69b-ba92a9ecaba2)

Apareixerà l'arxiu "NTUSER.DAT"

![image](https://github.com/user-attachments/assets/ec84076d-5e7e-41bb-8ef7-7193410c4338)

Canviem l'extensió del fitxer a ".MAT"

![image](https://github.com/user-attachments/assets/3cff2506-4ad8-47fd-9d56-19b9cbed6cb1)

## Pas 3 - Modificar la carpeta del perfil a l'usuari

Anem a l'usuari que hem escollit i obrim "propiedades"

![image](https://github.com/user-attachments/assets/8f9a973c-4be9-48b3-adea-9944dd185275)

Anem a la pestanya "Perfil"

![image](https://github.com/user-attachments/assets/5c5839e0-fb8e-4d2e-9b52-b1dca4519412)

Escrivim la ruta a la carpeta Perfiles del servidor i afegim la variable d'entorn "%username%"

![image](https://github.com/user-attachments/assets/7ef12c8e-e0e9-4802-b3da-32e54f62cc91)

## Pas 4 - Inici de sessió al client

Iniciem sessió al client per obtenir un meravellós ERROR CRÍTIC

![Uploading image.png…]()





