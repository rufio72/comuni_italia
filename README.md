# Comuni italia sql (mysql)
elenco comuni -> province -> regioni | Esportazione da mysql

Il file comuni.sql è un database con dentro 3 tabelle, rispettivamente: comuni, province e regioni.
I dati li ho presi dal sito dell'istat e sembrano aggiornati al 7 luglio 2020. (Non so se sia vero, ma è molto probabile)

I file che ho scaricato sono presenti, nel progetto, nella cartella dati_istat, che contiene il file excel e un file csv che ho usato per l'importazione.
Nella tabella comuni, tra gli altri, sono presenti 2 campi nominati id_provincia e id_regione, legati rispettivamente agli id della tabella province e regioni.

Invece nella cartella old è presente la vecchia esportazione.
Quest'ultima l'avevo generata da un progetto opensource che era aggiornato al 2018, modificato in modo da facilitare le query.
Questo è il progetto open-source che a suo tempo ho vampirizzato: https://github.com/MatteoHenryChinaski/Comuni-Italiani-2018-Sql-Json-excel

# Struttura database

## Tabella regioni
 
**id** -> autoincrement unica 

**codice** -> codice numerico rappresentativo della regione

**nome** -> nome della regione

## Tabella Province

**id** -> autoincrement unica

**id_regione** -> Campo id della tabella regioni, serve a ricavare le provincie di una certa regione

**codice** -> codice alfanumerico assegnato alla provincia

**nome**   -> nome della provincia

**sigla**  -> sigla automobilistica della provincia


## Tabella comuni
Questa tabella è frutto dell'importazione della tabella comuni scaricata dall'istat




Happy download!

Link per scaricare il file excel direttamente dal sito istat.
https://www.istat.it/storage/codici-unita-amministrative/Elenco-comuni-italiani.xls

