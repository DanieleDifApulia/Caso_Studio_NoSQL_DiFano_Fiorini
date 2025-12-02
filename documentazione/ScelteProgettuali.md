# Scelta Progettuali per il Db

---
Le prinicipali scelte progettuali sono state :

## Aeroporto { Terminal { Gate } } Emb

La scelta di unire i Gate a Terminal , Terminal in Aeroporto per seguire il pattern progettuale

Entità "Contenuta" in Entità 

In oltre per la bassa frequenza di aggiornameto dei dati.

## Volo Programmato  1 -> N Prenotazioni  Ref

Abbiamo referenziato le due collection per non appesantire il Documento dell' Volo Pr.
Con tutte le informazioni delle prenotazioni 

## Prenotazioni 1 -> Biglietti Ref

Abbiamo referenziato le due collection per non appesantire il documento del biglietto per 
eventuali controlli del personale aeroportuale e tenere le due entità separate.

## Biglietto { Passeggiero } Emb

Abbiamo optato di inserire di dati del passeggiero nel biglietto per seguire il pattern progettuale

Entità "Contenuta" in Entità.

## Compagnia 1 -> N Aereomobili Ref

Abbiamo optato di referenziare per le possibili cambi contrattuali di un aeromobile con le compagnie 
in oltre abbiamo ipotizzato che un aromobili può essere affittato a una solo compagnia alla volta 
in oltre per non appesantire il documento aeromobile e tenerlo separato.


