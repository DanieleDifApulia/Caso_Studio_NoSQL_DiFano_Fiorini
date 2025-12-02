# Aereoporto:
---
#### NomeAereoporto
    Identificativo alfanumerico univoco dell'aereoporto - String (e.g. "John F. Kennedy International Airport")
#### IATA3
    Identificativo alfanumerico a 3 lettere univoco per aereoporti - String (e.g. "JFK")
#### FusoOrario
    Identificativo alfanumerico di zona oraria a 3/4 lettere, ignorato l'offset UTC - String (e.g. "EST")
#### Coordinate
    Dato composto da LAT e LONG che indica la posizione geografica dell'aereoporto - String (e.g. "40.6446° N, 73.7797° W")
#### LAT
    Coordinata alfanumerica geografica di latitudine - String (e.g. "40.6446° N")
#### LONG
    Coordinata alfanumerica geografica di longitudine - String (e.g. "73.7797° W")
#### Terminal
    Identificativo numerico per infrastrutture di imbarco, sbarco, check-in e ritiro bagagli - int (e.g. "1")

# Gate:
---
#### NumGate
    Identificativo numerico per infrastruttura di appoggio alle piste - int (e.g. "3") 
#### ***Terminal***
###### *Vedi **Aereoporto - Terminal***
#### Stato
    Stato alfanumerico attuale di operazione del gate - String (e.g. "Disponibile")

# Compagnia:
---
#### NomeCompagnia
    Identificativo alfanumerico univoco della compagnia - String (e.g. "RyanAir Ltd.")
#### IATA2
    Identificativo alfanumerico a 2 lettere univoco per compagnie aeree - String (e.g. "FR")
#### Sede
    Identificativo alfanumerico univoco della sede legale della compagnia - String (e.g. "Irlanda")
#### Alleanza
    Identificativo alfanumerico univoco dell'alleanza di appartenenza della compagnia - String (e.g. "SkyTeam")

# Aereomobile:
---
#### Modello
    Identificativo alfanumerico univoco dell'aereomobile - String (e.g. "747")
#### Produttore
    Identificativo alfanumerico univoco dell'azienda di produzione dell'aereomobile - String (e.g. "Boeing")
    