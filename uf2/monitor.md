# Monitoritzar Linux

![image](https://github.com/XaSaFa/MP04/assets/110727546/032697e9-bca3-4b8c-9182-17417d4911f6)

El monitoratge del sistema ens serveix per evitar caigudes de rendiment i tenir una alta disponibilitat del sistema.

Normalment es busca trobar si hi ha algun problema de rendiment a:

- Memòria.
- Processos.
- Emmagatzematge.
- Connexions de xarxa.

Hi ha una serie de comandes que ens serveixen per a fer-ho:

## top

La comanda top és una comanda que normalment va integrada a les distribucions Linux, ens mostra el grau d'ocupació de la CPU, la memòria RAM, la memòria d'intercanvi (SWAP) i els processos que s'estan executant.

![image](https://github.com/XaSaFa/MP04/assets/110727546/c1db49cf-f9a7-428c-9dcf-43dbe388d6f7)

### Estat del sistema

#### Informació

![image](https://github.com/XaSaFa/MP04/assets/110727546/383af85a-7967-4d72-b7b6-a9e7d7d3749c)

El primer número ens mostra el temps (la hora), up ens indica quan temps fa que està funcionant el SO i user és la quantitat d'usuaris connectats.

#### Memòria

![image](https://github.com/XaSaFa/MP04/assets/110727546/44b0e959-f737-43cd-a10b-fb13cf032eaf)

Aquest quadre ens indica la memòria del sistema: total, lliure, utilitzada i en búfer).

#### Processos

Els processos es mostren en aquesta secció:

![image](https://github.com/XaSaFa/MP04/assets/110727546/2a17fa22-f9a4-4585-bece-eb7f8acfe9a8)

Els processos running són els que estan en execució, sleeping són els que estan esperant una informació d'un procés d'entrada/sortida o un event per seguir executant-se.

Els processos stopped són processos que s'han aturat (per exemple amb un control+Z), els processos zombie són processos fills que estan pendents de que el procés que els ha creat els recuperi en algun moment.

#### Estat dels processadors

L'estat dels processadors també es mostra amb top:

![image](https://github.com/XaSaFa/MP04/assets/110727546/e242d410-d601-4e24-bf18-bb5b348f722d)

us mostra el temps emprat amb processos dels usuaris, sy mostra temps emprat amb processos del sistema.


### Ordenar processos

Si presionem h durant l'execució de top ens surten les opcions que té el programa, per exemple ens deixa ordenar els processos per la càrrega de CPU o la memòria que ocupen.

![image](https://github.com/XaSaFa/MP04/assets/110727546/3177575e-9a20-478f-ab26-67d2f16e17a0)

### Veure els processos d'un únic usuari

Dins de top puc utilitzar la lletra u per filtrar procesos d'un usuari concret.

Per exemple amb u xavi només mostrarà els processos de l'usuari xavi:

![image](https://github.com/XaSaFa/MP04/assets/110727546/45bc76d8-18f1-4e88-aa68-9d52dcb44b76)

Per tornar a veure tots els processos prenem la lletra u i enter.

Podem fer el mateix si per terminal introduïm la instrucció ``` top -u usuari ```

### Matar un procés

Si tinc un procés que vull parar, com el de l'exemple següent (Firefox), simplement he d'introduïr la lletra k (kill) i el número PID del procés, en aquest cas 3191.

![image](https://github.com/XaSaFa/MP04/assets/110727546/b534adaa-a7c7-41e6-88c9-b6c79d3bf429)

![image](https://github.com/XaSaFa/MP04/assets/110727546/439645bc-8885-42e8-9b4f-8b896c67b778)

Això envia una senyal al procés per a tancar-ho.
