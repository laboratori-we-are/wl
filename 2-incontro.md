# Diario 2. incontro

Obiettivo: Familiarizzare con Wikibase e la gestione delle ontologie


## Lavoro in laboratorio

### Creazioni di *elementi* (item) e di *proprietà*

* [elementi](https://smartmeta.wiki.opencura.com/wiki/Special:AllPages?from=&to=&namespace=120)
* [proprietà](https://smartmeta.wiki.opencura.com/wiki/Special:AllPages?from=&to=&namespace=120)

### Primo tentativo:   un *video*

[Luci e ombre del Semantic Web](https://smartmeta.wiki.opencura.com/wiki/Item:Q8)

*  le proprietà di tipo URL ora funzionano (https://smartmeta.wiki.opencura.com/wiki/Property:P6)
* le proprietà che prevedono una tipologia di dato *testo monolilngua*  non sono indicizzate come full-text
* ho creato la proprietà *titolo_s* con tipologia di dato *stringa* e la *lingua* (italiano/inglese) la ho aggiunta come *qualificatore*
* tutte le *stringhe* contenute nelle *dichiarazioni* (*statements*) **e**  *Etichetta+Descrizione+Alias* sono ricercabili come *full-text*  
* Quando si cerca  nel campo di ricerca in testa alla pagina "Cerca in Metadati intellligenti"
	*  funziona il completamento automatico della *Etichetta*  (ricerca per inizio *Etichetta* : es cominciare a scrivere *luc*)
	* è possibile anche  la ricerca full text per il testo contenuto su tutte le *stringhe* contenute nelle *dichiarazioni* (*statements*) **e**  in *Etichetta+Descrizione+Alias* sono ricercabili come *full-text*  con le convenzioni che seguono (senza la pretesa di elencarle tutte) :
		* parola intera (es *shadows* oppure *seminario*)
		* più parole (es *shadows lights*)
			* \\? per indicare un carattere mancante in qualsiasi posizione (es *light\\?*)
			* \* per indicare più caratteri mancanti in qualsiasi posizione (es *\*ghts*)

### idee da provare prima del 3. incontro
(modificate, aggiungete, cancellate senza problemi)

* LRM proposta Stefano 
*  gerarchia delle entità LRM -tabella 4.1?- (Denise)
* Agent e dintorni (Valentina)
* ontologia cartoline (Marina)
* tutti si possono aggiungere alle proposte esistenti e farne altre