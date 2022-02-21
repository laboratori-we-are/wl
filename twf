#### 3. incontro e compiti a casa

Con  il 3. incontro abbiamo raggiunto davvero il punto più difficile del  Lab4. 

Abbiamo cercato di gestire l'ontologia LRM e le relative istanze con il  metamodello di dati wikibase.

Tutto è andato abbastanza bene fino a quando siamo arrivati al *nomen*. Siamo stati assaliti tutti da molti dubbi ( tra il dire e il fare succede)

La nostra implementazione è stata tuttavia corretta. 

Qui sotto trovate quanto Pat Riva scrive a proposito del *nomen*

«L’entità *nomen* è sicuramente la più astratta delle entità in IFLA LRM. Le istanze dell’entità *nomen* vengono create applicando la relazione \<ha per appellativo\> (LRM-R13) a un’istanza di *res*.
Una volta creata un’associazione fra l’entità che è nominata e il nome utilizzato per essa, quella relazione diventa il *nomen*. Nella definizione per l’entità *nomen* questo concetto si esprime come segue:
*Un’associazione tra un’entità e un nome che si riferisce a essa*.
I vincoli, o cardinalità, della relazione \<ha per appellativo\> derivano da questa definizione:
> 1. Ogni *nomen* è associato a una e una sola *res*.
> 2. Ogni *res* può avere diversi *nomen*.
> 3. Una *res* deve avere almeno un *nomen* perché sia identificata e si possa fare riferimento a essa.»

Dato che tutte le entità sono sottoclassi di *res*,  tutte le istanze delle entità  (Opera, Espressione, Manifestazione, Agente) **devono** avere almeno un *nomen*.

Questa la spiegazione - sempre di Pat Riva - della **necessità del nomen** nel modello LRM

«Nella terminologia della modellizzazione, un *nomen* è una
relazione reificata. La reificazione si impiega nella modellizzazione per permettere che un’associazione si comporti come un’entità perché possa a sua volta avere attributi e partecipare a relazioni ulteriori. Questo metodo si applica bene all’entità *nomen*, perché nell’universo bibliografico ci interessa molto registrare gli attributi
delle istanze dei *nomen* e le relazioni fra i *nomen*. Questa è una parte importante della funzione dei nostri file d’autorità, nonché una componente essenziale dei database bibliografici.»

Questo complica un po' le cose sia come inserimento dei dati, sia come usabilità del  sistema (l'astratezza dell'entità *nomen* pesa).

Nella ricerca di altre sperimentazioni LRM ci siamo imbattuti  in un  recente articolo *Prototype Cataloging Interface Based on the IFLA Library Reference Model (LRM). Part 1: Conceptual Design / Mihela Pauman Budanović & Maja Žumer*  <https://www.tandfonline.com/doi/full/10.1080/01639374.2021.1974633?scroll=top&needAccess=true>
