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
#### ListaTerminal<>
    Lista dei terminal compresi nell'aereoporto e i loro dati - list (e.g. "Terminal 1, imbarco, gate 1")
#### Terminal
    Identificativo numerico per infrastrutture di imbarco, sbarco, check-in e ritiro bagagli - int (e.g. "1")
#### TipoTerminal
    Tipologia in uso del terminal - String (e.g. "imbarco")

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
#### AnnoProduzione
    Identificativo tipo data dell'anno di produzione dell'aereomobile - date (e.g. "1992")
#### Capacità
    Identificativo numerico di capacità totale dell'aereomobile - int (e.g. "90")

# Voli:
---
#### Tipo
    Tipo del volo, programmato o operativo - String
#### NumVP
    Identificativo numerico del volo programmato - int (e.g. "147")
#### *PartenzaVP*
    Aereoporto di partenza del volo programmato, referenza a IATA3
#### ArrivoVP
    Aereoporto di arrivo del volo programmato, referenza a IATA3
#### GiorniOperativi
    Descrizione dei giorni della settimana di operazione del volo programmato - String (e.g. "Lunedì - Giovedì")
#### OrarioPartenzaVP
    Orario di partenza del volo programmato - date (e.g. "13:00")
#### OrarioArrivoVP
    Orario di arrivo del volo programmato - date (e.g. "17:00")
#### DurataVP
#### DataVO
#### StatoVO
#### GateVO
#### AereoVO
#### PersonaleVO