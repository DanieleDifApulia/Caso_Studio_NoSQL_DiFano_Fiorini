Aeroporto:
---
#### NomeAeroporto
    Identificativo alfanumerico univoco dell'aeroporto - String (e.g. "John F. Kennedy International Airport")
#### IATA3
    Identificativo alfanumerico a 3 lettere univoco per aereoporti - String (e.g. "JFK")
#### FusoOrario
    Identificativo alfanumerico di zona oraria a 3/4 lettere, ignorato l'offset UTC - String (e.g. "EST")
#### Coordinate
    Dato composto da LAT e LONG che indica la posizione geografica dell'aeroporto - String (e.g. "40.6446° N, 73.7797° W")
#### LAT
    Coordinata alfanumerica geografica di latitudine - String (e.g. "40.6446° N")
#### LONG
    Coordinata alfanumerica geografica di longitudine - String (e.g. "73.7797° W")
#### ListaTerminal<>
    Lista dei terminal compresi nell'aeroporto e i loro dati - list (e.g. "Terminal 1, imbarco, gate 1")
#### Terminal
    Identificativo numerico per infrastrutture di imbarco, sbarco, check-in e ritiro bagagli - int (e.g. "1")
#### TipoTerminal
    Tipologia in uso del terminal - String (e.g. "imbarco")

Gate:
---
#### NumGate
    Identificativo numerico per infrastruttura di appoggio alle piste - int (e.g. "3") 
#### ***Terminal***
###### *Vedi **Aeroporto - Terminal***
#### Stato
    Stato alfanumerico attuale di operazione del gate - String (e.g. "Disponibile")

Compagnia:
---
#### NomeCompagnia
    Identificativo alfanumerico univoco della compagnia - String (e.g. "RyanAir Ltd.")
#### IATA2
    Identificativo alfanumerico a 2 lettere univoco per compagnie aeree - String (e.g. "FR")
#### Sede
    Identificativo alfanumerico univoco della sede legale della compagnia - String (e.g. "Irlanda")
#### Alleanza
    Identificativo alfanumerico univoco dell'alleanza di appartenenza della compagnia - String (e.g. "SkyTeam")

Aeromobile:
---
#### VIN
    Identificativo alfanumerico di registrazione dell'aereomobile di 17 cifre - String (e.g. "1FDWE37S5WHB43777")
#### Modello
    Identificativo alfanumerico univoco dell'aereomobile - String (e.g. "747")
#### Produttore
    Identificativo alfanumerico univoco dell'azienda di produzione dell'aereomobile - String (e.g. "Boeing")
#### AnnoProduzione
    Identificativo tipo data dell'anno di produzione dell'aereomobile - date (e.g. "1992")
#### Capacità
    Identificativo numerico di capacità totale dell'aereomobile - int (e.g. "90")

VoloProg:
---
#### Tipo
    Tipo del volo, programmato o operativo - String
#### NumVP
    Identificativo alfanumerico del volo programmato - String (e.g. "AZ147")
#### PartenzaVP
    Aeroporto di partenza del volo programmato, referenza a Aeroporto - IATA3
#### ArrivoVP
    Aeroporto di arrivo del volo programmato, referenza a Aeroporto - IATA3
#### GiorniOp
    Descrizione dei giorni della settimana di operazione del volo programmato - String (e.g. "Lunedì - Giovedì")
#### OrarioPartenzaVP
    Orario di partenza del volo programmato - date (e.g. "13:00")
#### OrarioArrivoVP
    Orario di arrivo del volo programmato - date (e.g. "17:00")
#### DurataVP
    Durata stimata del volo programmato - String (e.g. "3:30")

VoloOp
---
#### NumVO
    Identificativo alfanumerico del volo operativo - String (e.g. "AZ147")
#### DataVO
    Data del volo operativo, unix timestamp - int (e.g. "1764670528)
#### StatoVO
    Stato del volo operativo - String (e.g. "Partito")
#### GateVO
    Gate assegnato al volo operativo, referenza a Gate - NumGate
#### AereoVO
    Aereomobile assegnato al volo operativo, referenza a Aereomobile - VIN

Personale:
---
#### Matricola
    Identificativo alfanumerico del membro del personale - String (e.g. "AD-4532")
#### Nome
    Nome del membro del personale - String (e.g. "John")
#### Cognome
    Cognome del membro del personale - String (e.g. "Pork")
#### Ruolo
    Ruolo del membro del personale - String (e.g. "Pilota")


Prenotazione:
---
#### NomePagante
    Nome del Pagante della prenotazione
#### CognomePagante
    Cognome del Pagante della prenotazione
#### IdPrenotazione
    Id della Prenotzione
#### StatoPren
    Descrizione alfanumerica dello stato della prenotazione - String (e.g. "Cancellata")
#### Classe
    Descrizione alfanumerica classe prenotata dal cliente - String (e.g. "1a")

Biglietto:
---
### Passeggero:

    Nome
        Nome del passeggero - String (e.g. "Gaetano")
    Cognome
        Cognome del passeggero - String (e.g. "Cascione")
    DataNascita
        Data di nascita del passeggero - date (e.g. "06/02/2004")
    PNR
        Passenger Name Record, codice identificativo alfanumerico di 6 carattare - String (e.g. "P52DKC")

#### NumB
    Numero del biglietto - int (e.g. "123948")
#### IdPrenotazione
###### *Vedi **Prenotazione - IdPrenotazione***
#### VoloB
    Identificativo volo del biglietto, referenza a VoloOp - NumVO




