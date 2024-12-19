Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario

| Name | type | Attributes | Note
| Targa | VARCHAR(25) | NOT-NULL PRIMARY KEY | varchar(20) perchè in 20 caratteri si possono rappresentare (penso) tutte le targe comprese le personallizate
| Marca | VARCHAR(25) | NOT-NULL
| Modello | VARCHAR(50) | NOT-NULL
| Cambio_manuale | BOOLEAN | NOT-NULL
| Carburante | VARCHAR(20) | NOT-NULL
| Cavalli | TINY_INT | NOT-NULL UNSIGNED
| Colore | VARCHAR(20) | NOT-NULL
| Chilometraggio | MEDIUM_INT | NULL Default(NULL) UNSIGNED | NULL perchè una macchina può essere nuova e non avere chilometri (mi sale il dubbio se utilizzare NULL o NOT_NULL DEFAULT(0))
| Condizione | VARCHAR(15) | NOT-NULL | Esempio : nuovo, quasi nuovo, usato, malandato
| Data_acquisto | DATE | NULL | se è stata acquistata direttamente dalla concessionaria per la vendita al cliente(quindi è nuova) come data di acquisto si può considerare l'anno di fabbricazione
| Anno_fabbricazione | YEAR | NOT-NULL
| Prezzo | DECIMALE(8,2) | NOT-NULL
| Garanzia | BOOLEAN | NULL DEFAULT(NULL)
| Scadenza_garanzia | DATE | NULL
