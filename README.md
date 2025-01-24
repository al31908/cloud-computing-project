# cloud-computing-project

# Progetto: Applicazione Distribuita - Libretto Universitario

Questo progetto consiste nella realizzazione di un'applicazione distribuita che simula un libretto universitario digitale. Gli utenti possono registrarsi tramite email, effettuare il login e gestire i propri esami in una tabella personalizzata. 

## Descrizione del progetto

L'obiettivo del progetto era creare un'applicazione distribuita utilizzando Docker per la distribuzione e Kubernetes per l'orchestrazione e la gestione del carico delle richieste. 

Il processo di sviluppo ha seguito un approccio incrementale:
1. **Sviluppo locale**: L'applicazione è stata inizialmente realizzata e testata completamente in locale per garantire una base stabile e funzionante.
2. **Distribuzione**: Successivamente, sono stati implementati Docker e Kubernetes per distribuire e orchestrare i vari componenti dell'applicazione.

## Funzionalità principali

- **Registrazione e login**: Gli utenti possono registrarsi con la propria email e successivamente accedere al sistema.
- **Gestione degli esami**: Una volta effettuato l'accesso, è possibile aggiungere, visualizzare e gestire i propri esami all'interno di una tabella interattiva.
- **Interfaccia intuitiva**: L'applicazione è stata progettata per essere semplice da usare, con un'interfaccia chiara e accessibile.

## Architettura dell'applicazione

L'applicazione è composta da tre principali componenti:

### 1. **Frontend**
- **Tecnologia**: [React](https://reactjs.org/)
- **Descrizione**: Il frontend è responsabile dell'interfaccia utente. Offre un'interazione semplice e diretta per l'utente, consentendo la gestione del libretto universitario.

### 2. **Backend**
- **Tecnologia**: [Node.js](https://nodejs.org/)
- **Descrizione**: Il backend gestisce la logica applicativa e funge da intermediario tra il frontend e il database. Le chiamate tra frontend e backend sono state implementate tramite API RESTful.

### 3. **Database**
- **Tecnologia**: [Datastax Astra DB](https://www.datastax.com/astra) con Cassandra
- **Descrizione**: Il database, già in cloud, viene utilizzato per memorizzare i dati degli utenti e degli esami.

## Distribuzione e orchestrazione

- **Docker**: Ogni componente dell'applicazione (frontend, backend) è stato containerizzato tramite Docker, garantendo un ambiente di esecuzione portabile e uniforme.
- **Kubernetes**: Kubernetes è stato utilizzato per orchestrare i container, bilanciare il carico delle richieste e garantire la scalabilità dell'applicazione.




