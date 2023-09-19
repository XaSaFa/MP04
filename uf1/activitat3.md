# Activitat 3 - Instal·lació de Windows Server 2016

**OBJECTIUS DE L'ACTIVITAT**

Conèixer i documentar la instal·lació d'un Windows Server en mode d'escriptòri.

**MATERIAL NECESSARI**

- Una imatge ISO de Microsoft Windows Server 2016 instal·lable o els arxius d'instal·lació.
- El software de virtualització Virtual Box.
- Un processador de text per documentar el procés d'instal·lació.

**TASQUES A REALITZAR**

**MOLT IMPORTANT:**  Recorda que hauràs de documentar tot el procés. Fes les captures de pantalla i pren les notes que consideris necessàries.

1. Crea una màquina virtual amb els requisit mínims per instal·lar el Windows Server amb experiència d'escriptori indicat i aquests paràmetres:

Crea un nou disc dur de la mida recomanada (50 GB).
Utilitza el mètode d’emmagatzematge amb expansió dinàmica.
128 MB de memòria de vídeo.
Crea 2 targes de xarxa:
NAT
Xarxa interna (amb nom "intnet")

2. Realitza la instal·lació de Windows Server a la MV seguint les següents indicacions:

Tria la versió Estàndard amb Experiència d'Escriptori.
Instal·la les "Guest Additions" de Virtual Box.
Canvia les dades de l’equip a les següents:
Contrasenya de l’administrador: Qwerty1
Nom de l’equip: SVR-NomCognom (p.e. SVR_JosepRovira)
Tria la versió Estàndard amb Experiència d'Escriptori.
Fes que el servidor no sigui membre de cap domini i que sigui membre del
grup següent: IABSMX2.
Paràmetres de la xarxa interna (intnet):
IP: 192.168.XX.10/24 on XX és el teu número d'ordre al llistat d'alumnes.
DNS: 192.168.XX.10
Porta d'enllaç: 192.168.XX.10
Paràmetres de la xarxa NAT
Fer servir DHCP.

3. Documentació.

4. Crea un document de text que inclogui com a mínim (però no necessàriament limitat) els següents apartats:

- Portada: Instal·lació de Windows Server 2016 a una MV.
  
- Índex.
  
- Característiques del software.
  - Nom.
  - Propòsit o tipus d'aplicatiu.
  - Versió/compilació.
  - Requisits mínims/recomanables.
    
- Entorn d'instal·lació
  - Característiques de la màquina amfitrió (CPU, RAM, GPU, HDD, SO)
  - Característiques de la màquina hoste (Threads assignats, RAM, memòria de video, espai de disc)
    
- Procediment d'instal·lació.
  - Indiqueu tots els passos de la instal·lació des de el moment en que poseu la imatge a la unitat òptica virtual.
  - Feu una entrada per cada quadre de diàleg o interacció amb l'instal·lador.
  
- [Opcional] Troubleshooting: informa dels problemes que hagis detectat durant la instal·lació i les solucions que has fet servir.

- Proves de funcionament: Verificacions que has fet per comprovar que tot funciona correctament.
  - Configuració del servidor.
  - Configuració de xarxa.

**ENTREGA DE L'ACTIVITAT**

- Instal·lació de l'aplicació:

El mestre/a verificarà que heu fet la instal·lació correctament i us facilitarà una paraula clau.
Un cop la tinguis, introdueix la paraula clau al text de la tramesa.

- Documentació:

Adjunta el document resultant en format PDF a la  tasca de Classroom corresponent.

**VALORACIÓ DE L'ACTIVITAT**

- Instal·lació: 5 punts si s'han seguit tots els passos i tant la màquina com el sistema estan correctament configurats. 0 punts en qualsevol altre cas.

- Documentació: 5 punts en funció de la qualitat de la documentació, si s'ha arribat a fer els mínims.
