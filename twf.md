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

Nella ricerca di altre sperimentazioni LRM ci siamo imbattuti  in un  recente articolo *Prototype Cataloging Interface Based on the IFLA Library Reference Model (LRM). Part 1: Conceptual Design / Mihela Pauman Budanović & Maja Žumer*  <https://www.tandfonline.com/doi/full/10.1080/01639374.2021.1974633?scroll=top&needAccess=true> dove si legge «Of the eleven LRM entities: work, expression, manifestation, item, agent, person, collective agent, Res, nomen, place, and time span, the cornerstone are entities work, expression, manifestation, and item (see Table 1), their attributes and relationships, to which we focused in the design of our prototype cataloging interface »

In pratica hanno deciso di mettere su un prototipo LRM **senza** il *nomen*. La cosa è davvero strana dato che Maja Žumer è - con Pat Riva e Patrick Le Bœuf- una dei componenti del *FRBR Review group* che ha dato vita al modello LRM.  Il prototipo è destinato a catalogatori:  «the aim of this paper is to present a prototype cataloging interface, which provides easier data entry, follows the cataloger's thought process and is based on the advantages of the IFLA LRM model...».  Certo dimostrare i vantaggi di IFLA LRM **non** usando il *nomen* è davvero singolare.

Questo è uno dei primi risultati del Lab4: una sperimentazione seria del modello LRM con uno strumento tecnologicamente aggiornato e diffuso. Un grazie a Denise e a tutto il Lab4.

A questo punto riteneniamo che il percorso LRM  per quanto riguarda il Lab4 si possa fermare qui (naturalmente ognuno di noi se crede potrà continuare ad usare  *smartmeta* per approfondire LRM a livello personale.  È sicuramente una pista di studio molto interessante).  

Come  Lab4 è opportuno dedicare gli altri due incontri (3 bis e 4) ad altri percorsi, proprio per avere un quadro più generale delle possibilità di Wikibase. Ricordiamoci che il Lab4 ha l'obiettivo di dare delle linee guida per la presentazioni di progetti  "finanziabili" che prevedono l'uso di wikibase.

Il prossimo incontro sarà dedicato alle *cartoline* e come compito a casa vi proponiamo  l'inserimento di questa ontologia.

Esempio di riferimento per i dati
<https://www.rct.uk/collection/search#/1/collection/2955206/postcard-of-a-soldier-holding-an-envelope>

Ontologia proposta: <https://schema.org>
Fonte di riferimento per l'ontologia
<https://www.dataliberate.com/2019/04/03/something-for-archives-in-schema-org/>

Elementi base da inserire (tranne gli ultimi due)

| Entità | Tipo | Nota|
| --- | --- | --- |
|ArchiveComponent|Q|<https://schema.org/ArchiveComponent>|
|Collection|Q|<https://schema.org/Collection>|
|hasPart|P elemento|<https://schema.org/hasPart>|
|image|P url|<https://schema.org/image>|
|name|*non inserire*|<https://schema.org/image>|
|description|*non inserire*|<https://schema.org/image>|



