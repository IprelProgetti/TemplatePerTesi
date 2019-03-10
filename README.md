# TemplatePerTesi

Repository per tesisti, per archiviare in modo ordinato tutto il lavoro di tesi, monitorare lo stato di avanzamento ed essere supportati durante il percorso di tesi.

## Struttura

Ci sono quattro cartelle:

* **Articoli:** per archiviare i vari report sul lavoro svolto su base settimanale
	* `yyyy-mm-dd`: una cartella per ogni riunione settimanale
		* `week_X.md`: report settimanale scritto in Markdown
		* `resources`: cartella in cui inserire i multimedia per l'articolo Markdown
* **Codice:** conterrà tutto il codice sorgente della tesi
* **ToDo:** un file `weekX.txt` a settimana, in cui saranno inseriti gli assegnamenti per lo sprint successivo.
* **Letteratura:** cartella per archiviare le varie risorse bibliografiche della tesi (paper, conferenze, ricerche, ...)

## Metodologia di lavoro

Ogni tesista clonerà questo repository, rimuoverà il *remote* e lo sostituirà con quello del suo repository sul server Git aziendale.  
Il repository costituirà il nucleo del lavoro di tesi, su cui tutto dovrà essere salvato.

---

La `week0` costituisce la prima riunione, che si svolgerà il primo giorno del percorso di tesi. In essa verrà concordato il tema di tesi, la pianificazione temporale sugli obiettivi da raggiungere e gli step di lavoro iniziali.  
Il contenuto concordato verrà inserito nel file `ToDo/week0.txt`, che andrà a rappresentare la pianificazione del lavoro per la settimana successiva (la `week1`).

Durante la `week1` (*e in generale durante ogni settimana*) il tesista lavorerà alla sua tesi:

* archiviando i paper e ogni altra risorsa di interesse nella cartella `Letteratura`;
* committando il codice nella cartella `Codice`.

Al termine della settimana il tesista scriverà un breve articolo (o *report*) in Markdown di riassunto sull'attività svolta. Per la scrittura del report, attenersi alle seguenti linee guida:

* entrare nella cartella `Articoli`;
* **copiare** la cartella `yyyy-mm-gg` e **rinominare la copia** con la data di pubblicazione dell'articolo;
* entrare nella cartella così creata e rinominare il file `week_X.md` sostituendo alla lettera `X` il numero della settimana di lavoro;
* scrivere l'articolo:
	* seguendo il format di `week_X.md`, il quale costituisce il template per la scrittura;
	* inserendo in `resources` tutte le immagini, grafici, ... che saranno inserite nell'articolo.
* committare l'articolo e le sue risorse;
* loggarsi sulla propria sezione del blog aziendale `Tesi` e pubblicare un secondo articolo **copiando la sezione `Super Sintesi` e inserendo un link a `week_X.md` per l'accesso al contenuto dettagliato**.

> La cartella `Letteratura` è stata inizializzata con una breve guida introduttiva -- `IntroMarkdown.md` -- su come scrivere in Markdown).

La settimana si conclude con una riunione, in cui il tesista presenterà il suo lavoro settimanale utilizzando l'articolo come base per il suo discorso.

I tutor aziendali assisteranno alla presentazione, stabiliranno gli step di lavoro successivi e saranno disponibili per fornire consigli e supporto al tesista.

## Mutui vantaggi

#### Per il tesista:

* il suo percorso di tesi è seguito a stretto contatto dall'azienda;
* backup del progetto su Git;
* archiviazione ordinata della bibliografia;
* la successione dei vari articoli costituisce uno scheletro già pronto per la tesi di laurea.

#### Per l'azienda

* seguire da vicino il tesista e supportarlo frequentemente sulla base dello stato di avanzamento del suo lavoro;
* comprendere meglio le problematiche emerse e fornire maggiore supporto per la loro risoluzione;
* mantenere traccia del lavoro svolto dal tesista;
* imparare direttamente dal tesista dettagli sulle tecnologie usate.