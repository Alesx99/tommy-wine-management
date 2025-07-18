# 🚀 Setup e Installazione

Guida completa per configurare e utilizzare il sistema Gestione Tommy.

## 📋 Prerequisiti

- Browser moderno (Chrome, Firefox, Safari, Edge)
- Connessione internet per sincronizzazione (opzionale)
- Account GitHub per sincronizzazione (opzionale)

## 🔧 Installazione

### Metodo 1: Download Diretto

1. **Clona la repository**
   ```bash
   git clone https://github.com/Alesx99/tommy-wine-management.git
   cd tommy-wine-management
   ```

2. **Apri il file**
   - Doppio click su `index.html`
   - Si apre automaticamente nel browser

### Metodo 2: GitHub Pages

1. Vai su https://github.com/Alesx99/tommy-wine-management
2. Clicca su "Settings" → "Pages"
3. Seleziona "Deploy from a branch"
4. Scegli il branch "main"
5. Salva e attendi il deploy

## 🔐 Configurazione Iniziale

### Accesso al Sistema

1. **Apri l'applicazione**
   - Il modal di login apparirà automaticamente

2. **Scegli il tipo di accesso**
   - **Amministratore**: Username `Tommaso`, Password `Tommy123`
   - **Cliente**: Clicca "Accesso Cliente" per accesso guest

### Configurazione Sicurezza

1. **Cambia password di default**
   - Clicca il pulsante 🔒 "Sicurezza"
   - Inserisci password attuale: `Tommy123`
   - Inserisci nuova password
   - Conferma nuova password

2. **Configura timeout sicurezza**
   - La sicurezza si riattiva automaticamente dopo 5 minuti
   - Puoi modificare questo valore nel codice

## 📡 Configurazione Sincronizzazione GitHub

### Prerequisiti GitHub

1. **Crea un token GitHub**
   - Vai su GitHub.com → Settings → Developer settings
   - Clicca "Personal access tokens" → "Tokens (classic)"
   - Genera nuovo token con permessi `gist`
   - Copia il token (es: `ghp_xxxxxxxxxxxxxxxxxxxx`)

2. **Crea un Gist**
   - Vai su https://gist.github.com
   - Crea un nuovo Gist vuoto
   - Copia l'ID del Gist dall'URL

### Configurazione nel Sistema

1. **Accedi come amministratore**
   - Username: `Tommaso`
   - Password: `Tommy123`

2. **Configura GitHub**
   - Clicca il pulsante ⚙️ "GitHub" nell'header
   - Inserisci il token GitHub
   - Inserisci l'ID del Gist
   - Abilita la sincronizzazione
   - Clicca "Salva Configurazione"

3. **Testa la connessione**
   - Il sistema testerà automaticamente la connessione
   - Vedrai una notifica di successo

## 🎯 Primo Utilizzo

### Inserimento Dati

1. **Gestione Clienti**
   - Vai alla tab "👥 Clienti"
   - Compila il form con i dati del cliente
   - Clicca "➕ Aggiungi Cliente"

2. **Gestione Prodotti**
   - Vai alla tab "🍺 Prodotti"
   - Seleziona categoria e sottocategoria
   - Inserisci prezzi e quantità
   - Clicca "➕ Aggiungi Prodotto"

3. **Gestione Vini**
   - Vai alla tab "🍷 Vini"
   - Inserisci nome, produttore, annata
   - Seleziona tipologia e regione
   - Clicca "➕ Aggiungi Vino"

### Importazione Dati Esistenti

1. **Prepara file Excel**
   - Crea file Excel con le colonne corrette
   - Vedi sezione "Formato Dati" per dettagli

2. **Importa dati**
   - Clicca "📥 Importa Excel" nella sezione desiderata
   - Seleziona il file Excel
   - I dati verranno importati automaticamente

## 📊 Formato Dati Excel

### Clienti
```
Nome | Cognome | Email | Telefono | Indirizzo | Città | CAP | Data Registrazione | Note
```

### Prodotti
```
Nome | Categoria Principale | Sottocategoria | Marca | Prezzo Acquisto | Prezzo Vendita Ingrosso | Prezzo Vendita al Dettaglio | Quantità | Quantità Minima | Fornitore | Codice Prodotto | Note
```

### Vini
```
Nome | Produttore | Annata | Tipologia | Regione | Vitigno | Prezzo Acquisto | Prezzo Vendita Ingrosso | Prezzo Vendita al Dettaglio | Quantità | Unità di Misura | Fornitore | Codice Prodotto | Descrizione | Note
```

## 🔧 Personalizzazione

### Modifica Password di Default

Nel file `index.html`, cerca la riga:
```javascript
let SECURITY_PASSWORD = 'Tommy123';
```

Cambia `'Tommy123'` con la tua password.

### Modifica Timeout Sicurezza

Cerca la riga:
```javascript
setTimeout(() => {
    if (isSecurityUnlocked) {
        activateSecurity();
        showNotification('🔒 Sicurezza riattivata automaticamente', 'warning');
    }
}, 300000); // 5 minuti
```

Cambia `300000` con il tempo desiderato in millisecondi.

### Modifica Credenziali Admin

Cerca la funzione `validateLogin()` e modifica:
```javascript
if (username === 'Tommaso' && password === 'Tommy123') {
```

## 🚨 Risoluzione Problemi

### Problema: Dati non si salvano
- **Soluzione**: Verifica che il browser supporti localStorage
- **Test**: Apri console browser (F12) e digita `localStorage`

### Problema: Sincronizzazione non funziona
- **Soluzione**: Verifica token GitHub e Gist ID
- **Test**: Controlla console browser per errori API

### Problema: Export Excel non funziona
- **Soluzione**: Verifica connessione internet per CDN SheetJS
- **Test**: Ricarica la pagina

### Problema: Interfaccia non responsive
- **Soluzione**: Aggiorna browser a versione recente
- **Test**: Prova su Chrome/Firefox

## 📞 Supporto

Per problemi o domande:
1. Controlla la console del browser (F12)
2. Verifica la connessione internet
3. Prova su browser diverso
4. Controlla i log di errore

---

**🍷 Gestione Tommy** - Setup completato con successo! 