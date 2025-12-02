==================================================
CASO DI STUDIO: SISTEMA DI GESTIONE AEROPORTUALE
==================================================

Il caso di studio può essere svolto da un gruppo di massimo 3 persone.
Può essere svolto anche da soli.

DESCRIZIONE DEL DOMINIO
-----------------------

Un grande aeroporto internazionale intende rinnovare il proprio sistema
informativo utilizzando MongoDB come sistema di gestione dei dati. L'obiettivo
è progettare un database che supporti le operazioni quotidiane dell'aeroporto,
dalla gestione dei voli alla gestione del personale.

REQUISITI INFORMATIVI
----------------------

Il sistema deve gestire le seguenti informazioni:

AEROPORTI E INFRASTRUTTURE
- Ogni aeroporto è identificato da un codice IATA univoco (es. FCO, JFK)
- Nome completo dell'aeroporto, città e paese in cui si trova
- Fuso orario di riferimento
- Coordinate geografiche (latitudine e longitudine)
- I terminal presenti (Check-in, Imbarco, Sbarco, Ritiro Bagagli)

GATE
- Dei vari gate si vuole memorizzare: numero identificativo, terminal di appartenenza, stato
  operativo (disponibile, occupato, in manutenzione)

COMPAGNIA AEREA
- Codice IATA della compagnia (es. AZ, BA, LH)
- Nome commerciale completo
- Paese dove ha sede legale
- Eventuale alleanza di appartenenza (Star Alliance, SkyTeam, Oneworld)

AEREOMOBILE
Di un aeromobile si vuole memorizzare: numero di registrazione univoco, modello e produttore,
anno di produzione, capacità totale passeggeri


VOLI E PROGRAMMAZIONE
- Esistono voli "programmati" (es. il volo AZ123 che
  parte tutti i lunedì alle 10:00) e voli "operativi" (es. il volo AZ123
  specifico del 15 marzo 2024)
- Per i voli programmati bisogna memorizzare numero del volo, aeroporto di partenza e arrivo,
  giorni della settimana in cui opera, orari previsti di partenza e arrivo,
  durata stimata.
- Per i voli operativi: data specifica, stato attuale (schedulato, boarding, partito, in volo, atterrato, cancellato),
  gate assegnato, aeromobile utilizzato, personale a bordo con il relativo ruolo.

PASSEGGERI E PRENOTAZIONI
Dei passeggeri si vuole memorizzare
- Dati anagrafici: nome, cognome, data di nascita
- Per ogni prenotazione: codice PNR univoco, data in cui è stata effettuata
  la prenotazione, stato (confermata, check-in effettuato, completata,
  cancellata), classe prenotata
- Per ogni biglietto: numero univoco del biglietto, volo associato, passeggero
  intestatario, posto assegnato (numero e lettera, es. 12A)

PERSONALE
- Numero di matricola aziendale
- Nome e cognome
- Ruolo (pilota, primo ufficiale, assistente di volo, personale di terra,
  tecnico di manutenzione)


ATTIVITÀ RICHIESTE
---------------------

1. Documentare le scelte relative alle relazioni fra collections (Embedded / Referenziate) in un file Word o PowerPoint.
2. Scrivere in un file txt o markdown le insertMany che consentono di popolare le collections collegate alle due api
   (per chi sceglie la 4) ed inserirlo nella directory "scripts".
   Per chi sceglie la 4 inserire script del validator.

Scegliere una attività fra la 3 e la 4:
3. Scrivere un validator per almeno 2 collections usando o jsonSchema o gli operatori (a scelta)
4. Creare applicazione SpringBoot che esponga le seguenti api:

a) GET /flights/{flightId}
Output: dettagli del volo

b) GET /operational_flights
Output: dettagli di tutti i voli operativi

    (Non serve usare i DTO, potete restituire direttamente l'oggetto Document).

4. Pushare il progetto su GitHub. Nel repository creare la directory "documentazione" dove inserire il file (PowerPoint o Word)
   che spiega le decisioni e la directory "script" con i vari script per popolare il database.
   Nella documentazione scrivere nome e cognome del gruppo con cui si è svolto il caso di studio.

Se rimane tempo, potete:
- Creare altre api a vostro piacimento o validare altre collections.
- Usare i DTO al posto dei Document.
- Svolgere l'esercizio alternativo a quello che avete scelto per la 3/4.
