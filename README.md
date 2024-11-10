# Progetto_LAB_INF
Progetto esame Laboratorio d'Informatica 

# Piattaforma E-commerce per la Stampa di Gadget

## Panoramica
Questo sistema implementa le funzionalità principali di una piattaforma e-commerce specializzata nei servizi di stampa gadget. La piattaforma serve due tipologie di utenti:
- **Venditori**: Dipendenti dell'e-commerce che gestiscono prodotti e ordini
- **Clienti**: Aziende che utilizzano il servizio di stampa gadget

## Funzionalità

### Sistema di Autenticazione
- Registrazione utente per venditori e clienti
- Sistema di accesso sicuro con UserID e password
- Controllo accessi basato sui ruoli

### Funzionalità per i Clienti
1. **Gestione Ordini**
   - Effettuare nuovi ordini
   - Ricerca prodotti per nome (ricerca per sottostringa)
   - Aggiungere commenti agli ordini
   - Visualizzare lo storico degli ordini

2. **Statistiche Prodotti**
   - Visualizzare i gadget più venduti
   - Accedere ai dettagli e alla disponibilità dei prodotti

3. **Gestione Account**
   - Aggiornare le informazioni dell'account
   - Eliminare l'account
   - Funzionalità di logout

### Funzionalità per i Venditori
1. **Gestione Prodotti**
   - Aggiungere nuovi gadget
   - Modificare gadget esistenti
   - Rimuovere gadget dalla piattaforma

2. **Business Intelligence**
   - Visualizzare lo storico completo degli ordini
   - Accedere alla lista dei clienti registrati
   - Monitorare le performance dei prodotti

## Dettagli Prodotto
Ogni gadget nel sistema è caratterizzato da:
- Codice identificativo univoco
- Tipologia (Maglia, Tazza, Cappello, Penna, Portachiavi, Borraccia, Altro)
- Nome
- Colore
- Descrizione
- Prezzo
- Quantità in pronta consegna
- Numero di pezzi venduti
- Flag di stato eliminazione

## Elaborazione Ordini
- Generazione automatica ID ordine
- Controllo inventario in tempo reale
- Sistema di ordini a due stati:
  - Evasione diretta per prodotti disponibili
  - In attesa di approvazione per prodotti non disponibili

## Struttura Dati Utenti

### Profilo Venditore
- UserID (identificativo univoco)
- Password
- Cognome
- Nome

### Profilo Cliente
- UserID (identificativo univoco)
- Password
- Sede aziendale
- Nome azienda

## Note Tecniche
- Tutti gli UserID sono numeri interi positivi
- La ricerca prodotti implementa il matching per sottostringa
- Validazione automatica di tutti gli input
- Visualizzazione dati in formato tabellare

## Caratteristiche di Sicurezza
- Gestione sessioni con funzionalità di logout
- Autenticazione utente richiesta per tutte le operazioni
- Controllo accessi basato sui ruoli
- Possibilità di eliminazione account

## Flusso di Utilizzo
1. Messaggio di benvenuto all'avvio
2. Autenticazione utente (registrazione/login)
3. Visualizzazione menu specifico per ruolo
4. Esecuzione operazioni
5. Opzione di logout o continuazione
6. Possibilità di terminare il programma

## Persistenza Dati
- Tutti i dati dei prodotti sono memorizzati in modo persistente
- Lo storico degli ordini viene mantenuto
- Gli account utente sono preservati tra le sessioni
- Tracciamento dei prodotti eliminati per riferimento

Per maggiori informazioni o supporto tecnico, si prega di contattare l'amministratore di sistema.

---
*Nota: Questo sistema è progettato per operazioni business-to-business (B2B), specificamente rivolto ad aziende che richiedono servizi di stampa gadget personalizzati.*
