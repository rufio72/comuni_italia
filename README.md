# Comuni italia sql (mysql)
elenco comuni -> provincie -> regioni | Esportazione da mysql

Sono tre tabelle con dentro l'elenco dei comuni, provincie e regioni legate dai vari id.

L'ho preso da un progetto opensource che era aggiornato al 2018 e l'ho modificato in modo da facilitare le query.
Questo è il progetto open-source che ho preso come riferimento : https://github.com/MatteoHenryChinaski/Comuni-Italiani-2018-Sql-Json-excel

Nelle tabelle non trovavo le foreign key e non mi piace fare join partendo da campi varchar, quindi l'ho modificato. 

Questa è una pagina da cui è possibile scaricare l'elenco dei comuni italiani:
https://www.istat.it/storage/codici-unita-amministrative/Elenco-comuni-italiani.xls

Come vedete è una pagina dell'istat, quindi verrebbe da pensare che sia aggiornato.

Happy download!
