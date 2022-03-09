# Corso 1 Intro
# Week 1
# Data science
ci baseremo su R per esercizi come ulizia dei dati etc
La data science è in molti ambiti (sport, analisi dati industriali etc)
## Big Data
caratterizzati da 3 V

* Volume (Q.ta di dati disponibili)
* Velocity (generazione sempre >)
* Variety (i dati analizzati sono in differenti forme, i + complex sono img video bin etc) 

## Data
Aiutano alla decisione, influenza.
Variabili sono Quantitative (hanno a che fare con valori numerici) o qualitative (difficile raportarle)
Fluddo: prima la domanda, poi vedo cosa ho di rilevante nei dati.
In base ai dati vado a limare la domanda.

## Project  
* domanda
* esplora i dati (ML o statistica)
* comunica il proetto che vuoi fare
    * presentazione proj. etc


# Week 2
## R 
Linguaggio statistico 
## R packages
* lib: dove i pkg sono nel pc (libreria)
* pkg: collez. di dati e funzioni, codice pronti (libro)
Repository: dove i pkg sono salvati e disponibili per download.
## Project
per tenere i file organizzati insieme, è una folder e un {file}
R Studio li gestisce e li linka .rproject
* new project
* file new p
* project toolbar

# Week 3
## Version controll
* stage
* commit
* push
Esistono versioni online
Uso di key RSA

## Week 4
# Data science
5 tipi di problemi:
* Descrizione: descrivi un insieme di dati (riassunti, analisi di bnuovi dati etc) media, varianza etc non guida decisioni
* Esplorazione: esamino i dati per trovare relazioni (N.B. correlazione non implica causa effetto), mi concentro su nuove correlazioni per hp. future
* Inferenza: usa un numero limitato di osservazioni per dire qualcosa su larga scala (dal piccolo riesco a id feature che influenzano larghi gruppi)
* Predizione: usa dati storici per id pattern per il futuro, devo valutare quale variabili mi da predizioni più accurate per il caso (relaz + o - forti)
* Casualità: Cosa succede a una var se ne modifico un'altra è uno standard della data analysis, vanno fati casi appositi
* Mecannica: Identifica quali caratteristiche di una var. hanno influenza su caratt di un'altra (modellazione sistemi di eq. deterministiche) è per fisica e scienza (sistemi con noise esterna)
# Esperimental Design
Counfonder: variabile estranea che può influire sulla relaz. di altre 2 variabili con maggior # osservazioni possiao vedere quali variabili e come influiscono.
## Big Data
perchè se ne parla oggi? per lo sviluppo tecnologico: soprattutto velocità (q.to veloce posso catturare i dati) e volume (q.to è big) poi varietà (su cosa lavoro).
CI sono molti + formati, db spreadsheets etc, ora c'è molta + fruizione unstrutturata, video, audio, free text etc.
Avere molti dati aiuta perchè diminuisce l'influenza di outliers.
Big data rispondono a cosa? non a perchè? Non tutti i dataset sono utili alla tua domanda.

# Corso 2 r
# Week 1
## R
R deriva da S (ling dei bell labs per analisi statistiche). Eraun {lib fortran}, nel 88 viene riscritto con rutin in C
R nasce nel 91
Feature
* Syntax like S
* Quasi tutte le piattaforme
* Release frequenti
* package modulari e addizionali
* High lvl capacità grafiche
* comunity attiva
* Free
Cons
* 40 Anni
* grafica limitata (poco 3D)
* Obj sono memorizzati in meoria Fisica (lim alla dim)
* Non è general purpuse
R è diviso in "base" (utils, datasets... etc) + package addizionali

Assegnazione: x<-1
default X sarà un obj array con un valore : 1
i \# sono commenti in R
se metto nel terminale una variabile, di default sarà come farne la print
x <- 1:20 \# inserisce da 1 a 20 in x, a 16 va a un nuovo elem dell'array
## Data Types
5 basic:
* chaacter
* numeric (real): 2 cifre dopo la , tipo di default per i numeri kost importanti: inf e NaN
* integer
* complex
* logical (T o F)
Oggetti più complessi:
* Array/vettori (collez. di obj omogenei) : vector() creazione vettore vuoto oppure vector
* List simili a vettori, ma non c'è necessità di tipo omogeneo
Attributi: parti di un obj in R
esempi: nomi, class, dimensioni, length etc accesso a un attr. di un obj è con attributes()
## Vettori
Init. con c() o vector() se vuoto, dico il tipo
vettor <- c(val1,val2 ..., valn)
Se inserisco obj diversi in un vettore, viene fatta conversione tra i tipi primitivi (True -> 1 in numeri). Hanno singole parentesi
## List
ogni elem di una lista è di un tipo diverso, sono usati per combinare tipi diversi, quindi per ogni elem posso avere comportamenti diversi. Sono indicizzati, hanno doppie parentesi
## Matrici
Simili a vettori, ma hanno più dimensioni
x <- matrix(nrow=2, ncol=3)
dim(objmatrix) rit un vettore con info righe,colonne
posso anche definire come riempirla nel costruttore
m <- matrix(1:6 nrow=2, ncol=3)
## Factors
Vettori per rappresentare dati categorie: sono cat. ordinate o mno, sono come label che possono essere assegnate
creati con la funzione: factor()  a cui passo un vettore, se ci chiamo la funz. table sopra, mi dice quali sono le categorie (diverse) in un vettore fators.
nella creazione con level() posse def. un ordine delle label
## Missing Values
sono na o nan
nan: op matematiche non definite na: resto
is.na() e is.nan() funz. per check sugli obj
NaN è sottoinsieme di Na. 
## Dataframes
per dati tabulari, usati nella statistica etc.
sono delle liste speciali, in cui ogni elem della lista è una colonna, la length del singolo elemento è il # di righe.
ogni colonna ha un tipo omogeneo AL SUO INTERNO, le atrici sono completamente omogenee.
row.names attributo dei dataframes, sono creati tramite read.csv () o read.table() e possono essere convertiti in matrxi con data.matrix()
## Reading Data
read.table o read.csv leggono text file di tipo colonne e righe, rit un dataframe
readLines lettura di txt sequenziale
source è inverso di dump.



# Corso 3 Clening Data
## Week 1
I dati li trovo raw, diversi formati etc,  









1    41     190  7.4   67     5   1
2    36     118  8.0   72     5   2


21
37
