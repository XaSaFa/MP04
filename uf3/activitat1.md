# Activitat 1 - Permisos a Linux

1. Ves al teu directori personal i crea una carpeta anomenada "Exercici-X" on X és el teu cognom.
  - mkdir exercici-sancho

2. Canvia els permisos del directori perquè només el propietari tingui tots els permisos.

  - chmod 700 exercici-sancho/
3. Crea un arxiu anomenat "arxiu1.txt" dins del directori anterior i verifica els permisos.

  - cd exercici-sancho
  - touch arxiu1.txt
  - ls -l

4. Crea un grup anomenat "proves".

  - sudo addgroup proves
  
5. Dona-li permisos de lectura i escriptura sobre "arxiu1.txt" al grup.

  - sudo chown kal:proves arxiu1.txt

6. Crea un subdirectori anomenat "sub-X" on X és el teu cognom.

 - mkdir sub-sancho
  
7. Deixa el subdirectori anterior amb permisos només per al propietari (rwx).

  - chmod -R 700 sub-sancho/
  
8. Concedeix permisos d'execució al grup "proves" sobre "sub-X".

   - sudo chown kal:proves sub-sancho/
   - chmod 710 sub-sancho/

9. Crea un usuari anomenat "convidat".

   - sudo adduser convidat

10. Canvia els permisos del directori "Exercici-X" perquè l'usuari "convidat" pugui accedir.

  - chmod 701 exercici-sancho/

11. Canvia els permisos de l'arxiu "arxiu1.txt" perquè tots els usuaris tinguin només permís de lectura.

  - chmod 444 arxiu1.txt

12.  Comprova que l'usuari "convidat" no pot accedir al subdirectori "sub-X".

  - su convidat
  - ls -l

13.  Afegeix convidat al grup "proves" i comprova que sí té accés a "sub-X". (POTSER NECESSITES REINICIAR EL SISTEMA).
    
  - sudo addgroup convidat proves
  - chmod 750 sub-sancho/


# Activitat 2 - umask

1. Crea un usuari anomenat "proves2" i mostra la seva màscara per defecte.
2. Modifica la màscara de proves2 perquè els fitxers els crei amb rw-r--r-- i els directoris amb rwxr-xr-x.
3. Comprova que la màscara anterior funciona.
4. Modifica la màscara de proves2 perquè els fitxers els crei amb rw-rw-rw- i els directoris amb rwxrwxrwx.
5. Comprova que la màscara anterior funciona.
6. Modifica la màscara de proves2 perquè els fitxers els crei amb r--r--r-- i els directoris amb r-xr-xr-x.
7. Comprova que la màscara anterior funciona.
8. Modifica la màscara de proves2 perquè els fitxers els crei amb rw--w--w- i els directoris amb rwx--x--x.
9. Comprova que la màscara anterior funciona.
10. Modifica la màscara per crear un fitxer anomenat "511.txt" amb permisos r--------
11. Utilitza chmod perquè els permisos de "511.txt" siguin r-x--x--x.
12. Utilitza chmod perquè el fitxer anterior tingui permisos rwxrwxr-x.
13. Utilitza chown perquè el fitxer anterior sigui propietat de l'usuari root i del grup proves.
14. Intenta eliminar el fitxer amb l'usuari proves2. (sense sudo)
15. Afegeix l'usuari proves2 al grup proves i elimina el fitxer anterior.

16. 
