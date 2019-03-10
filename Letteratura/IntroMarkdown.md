# Introduzione a Markdown

Markdown è un linguaggio a marcatori (o markdown language) per scrivere testo.  
A differenza di HTML non richiede di inserire esplicitamente i tag in fase di scrittura, fatta eccezione per qualche simbolo per la formattazione del testo (dettagliati in seguito).

Nella scrittura, Markdown abbina la flessibilità di Word alla comodità di renderizzazione di HTML, risultando un ottimo compromesso per la distribuzione multi-piattaforma di file testuali. Il risultato è un file con estensione `.md`.

Oltre a poter essere visualizzato online all'interno delle apposite strutture contenitore (su tutti, i repository Git - che non mancano mai di un `README.md` - e i blog basati su WordPress), un file Markdown è leggero e convertibile istantaneamente in una vasta selezione di altri formati (su tutti: `.html`, `.pdf`, `.docx`, ...).

Per quest'ultimo scopo, è necessario un plugin esterno che funga da convertitore: [**Pandoc**](https://pandoc.org/index.html) è il più famoso.

## Come scrivere in Markdown

Al pari di ogni linguaggio a marcatori, per scrivere in Markdown non è necessario installare alcun software.  
Al contrario, è sufficiente aprire un classico blocco note, scrivere seguendo gli stili Markdown e salvare il tutto con estensione `.md`.

Per agevolare la scrittura, il consiglio è di utilizzare [Atom](https://atom.io) o [SublimeText](https://www.sublimetext.com) configurati con l'apposito pacchetto Markdown (il quale non aggiunge nient'altro che una finestra affiancata all'editor di testo in cui è renderizzato graficamente il testo scritto finora).

> **NB:** in Markdown non è possibile modificare l'allineamento del testo.  
> I documenti Markdown avranno tutti allineamento a sinistra.  
> Una volta esportati, tuttavia, il contenuto potrà essere gestito nei limiti consentiti dal nuovo formato (ad esempio, a valle della conversione da `.md` a `.docx` sarà possibile giustificare il testo).

Ecco un riferimento base per la scrittura in Markdown (ulteriori riferimenti [basici](https://www.markdownguide.org/basic-syntax) o [avanzati](https://www.markdownguide.org/extended-syntax) o [misti]((https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet))):

# Questo è un titolo

## Questo è un sottotitolo

### Questo è una intestazione più piccola

#### Ancora più piccola

##### Ancora più piccola

###### Titolo paragrafo

*parola in corsivo*  
**parola in grassetto**  
***parola in corsivo grassetto***

Per andare a capo, inserire due spazi dopo il punto e dare un singolo invio.  
Gli spazi sono importanti, se non vengono inseriti l'andare a capo con singolo invio sarà renderizzato comunque sulla stessa riga.
Provare per credere.

Un doppio invio genera un nuovo paragrafo.

* questa 
+ è
1. una
- lista
	- puntata
		* con rientranze
			+ multiple 

1. usare i numeri
2. per liste 
	3. che possono anche rientrare
		4. più
		5. volte	 
3. numerate  

> il simbolo > origina una zona per le citazioni  
> 
>> anche innestabili
>>> più volte  
>>
>> facilmente
>
> valgono tutte le regole
> 
> **già viste** 
> 
> * per
> * il
> * *testo*

Il `codice` può essere inserito `inline` (singolo backtick) o in blocco:

```
# blocco delimitato da tre backticks
def function_1(a):
	return a + 2
```

    # blocco originato scrivendo linee con 4 spazi iniziali
    def function_2(a):
        return a * 2

[parola da associare al link](https://www.google.it "Vai a google.it")     
<https://www.google.it>

![questa è una immagine](./logo.png)

| Esempio   | Tabella | Allineata |
| :---      | :---:   | --:       |
| Nome    | Allineati   | Sole   |
| Ciao | al    | mAre
| sinistra | centro | destra | 


## Esportare un file Markdown in altri formati

Tramite pandoc, su macOs, lanciare da terminale:

    $ pandoc -s -f markdown -t docx -o my_output_file.docx my_input_file.md
    
Per Windows, Linux o altri sistemi fare riferimento alla [documentazione](https://pandoc.org/MANUAL.html) ufficiale.