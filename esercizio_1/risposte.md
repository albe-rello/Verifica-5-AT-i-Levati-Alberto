1. Cos'è il DOM, struttura ad albero e specificità CSS
Cos'è il DOM e perché ha una struttura ad albero:
Il DOM (Document Object Model) è la rappresentazione logica e strutturata di un documento HTML creata dal browser in memoria. Permette ai linguaggi di programmazione (come JavaScript) e ai fogli di stile di accedere, modificare o interagire con gli elementi della pagina. Ha una struttura ad albero (detta tree structure) perché rispecchia fedelmente la natura gerarchica e nidificata dei tag HTML, dove un elemento (genitore) contiene altri elementi (figli).

Albero del DOM (fino al terzo livello):
html (Livello 1)
├── head (Livello 2)
│   ├── meta (Livello 3)
│   └── title (Livello 3)
└── body (Livello 2)
    ├── header (Livello 3)
    ├── nav (Livello 3)
    └── main (Livello 3)


2. Dalla digitazione dell'URL alla visualizzazione della pagina
Quando un utente digita l'indirizzo web (URL) e preme Invio, si attiva una sequenza di passaggi che coinvolgono tre componenti principali: Client (il browser dell'utente), DNS (Domain Name System) e Server (il computer remoto che ospita il sito).

Risoluzione DNS: Il browser controlla se conosce già l'indirizzo IP del dominio. In caso contrario, interroga i server DNS per tradurre il nome testuale del sito (es. ilmio-cinema.it) nell'indirizzo IP numerico del server di hosting.

Connessione e Richiesta (Client -> Server): Il browser (client) stabilisce una connessione di rete con il server tramite l'indirizzo IP ottenuto e invia una richiesta HTTP/HTTPS per ottenere la risorsa desiderata (solitamente index.html).

Elaborazione della richiesta (Server): Il server riceve la richiesta, individua i file del sito all'interno del proprio storage, li elabora e prepara il pacchetto di risposta.

Invio della risposta (Server -> Client): Il server restituisce al client il codice sorgente (HTML, CSS, immagini e script).

Rendering (Client): Il browser riceve i dati, interpreta l'HTML costruendo il DOM, applica il CSS, esegue il rendering grafico e mostra la pagina sullo schermo dell'utente.

3. Differenza tra git clone e git pull
git clone: Viene usato una sola volta per scaricare per la prima volta un repository remoto da una piattaforma come GitHub alla propria macchina locale. Crea una copia completa dell'intero progetto, compresa l'intera cronologia dei commit e tutti i branch.

git pull: Viene eseguito su un repository locale già esistente e già collegato a un remote. Serve ad aggiornare il proprio spazio di lavoro scaricando e unendo automaticamente le ultime modifiche pubblicate da altri sviluppatori sul repository remoto.