# Activitat 4 - Ús de diskpart

Entrega un pdf amb les solucions demanades, has de justificar les respostes amb text i imatges (captures de pantalla).

## Part 1 - Teoria.

Contesta les següents preguntes:

1. Investiga i explica les principals diferències entre discos durs HDD i SSD.
2. Quine diferències hi ha entre les taules de partició MBR i GPT?
3. Als equips actuals quina es fa servir? Justifica-ho amb hardware modern, mostrant les característiques de la placa base.
4. Quin és el tamany màxim d'una partició primària a GPT en GB?
5. Quin és el tamany màxim d'un disc a GPT en GB?
6. Si utilitzo Windows: Quantes particions màximes entre tots els tipus tindré en un disc dur amb taula MBR. Indica quantitat i tipus.
7. Investiga i explica breument què són els volums en mirall.
8. Investiga i explica breument què són els volums RAID-5.
9. Investiga i explica breument què són els volums distribuïts.
10. Investiga i explica breument què són els volums seccionats.

## Part 2 - Pràctica.

Mostra en tots els casos les captures de pantalla i si fa falta raona la resposta.

1. Crea un disc virtual de 10GB i afegeix-lo a la MV.

2. Crea 3 particions primàries que convertiràs a volums simples amb les següents característiques:
- Primera: Tamany de 1GB, lletra Z, etiqueta "Cognom-1".
- Segona: Tamany de 512MB, lletra X, etiqueta "Cognom-2".
- Tercera: Tamany de 2GB, lletra Y, etiqueta "Cognom-3".

3. Intenta crear una nova partició primària de 1GB. Què passa?

4. Crea una partició estesa amb la resta de disc dur, no et deixis res lliure.

5. Crea les següents particions lògiques:
- Primera: Tamany de 5GB, lletra W, etiqueta "Cognom-4".
- Segona: Tamany la resta, lletra V, etiqueta "Cognom-5".

6. Mostra els volums a l'explorador de Windows i al Panell d'administració del server.

7. Esborra el disc sencer.

8. Crea una partició primària de tamany de 3GB, lletra D, etiqueta "Cognom-1".

9. Amplia la partició fins a 9GB.

10. Redueix la partició 1024MB.

11. Crea una nova partició lògica que ocupi la resta del espai, lletra E, etiqueta "Cognom-2"

12. Mostra els volums a l'explorador de Windows i al Panell d'administració del server.
