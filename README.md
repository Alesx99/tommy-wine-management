# 🍷 Gestione Tommy - Sistema di Gestione Bar e Cantina

Sistema SPA (Single Page Application) per la gestione completa di un bar e cantina, con moduli per clienti, fatture, prodotti e vini.

## ✨ Funzionalità Principali

- **👥 Gestione Clienti**: Anagrafica completa con filtri e ricerca
- **📄 Gestione Fatture**: Controllo pagamenti e scadenze
- **🍺 Gestione Prodotti**: Catalogo con prezzi ingrosso/dettaglio
- **🍷 Gestione Vini**: Listino specializzato con stampa professionale
- **🔒 Sistema di Sicurezza**: Protezione prezzi di acquisto con password
- **📡 Sincronizzazione**: Supporto GitHub Gist per multi-dispositivo
- **📊 Export Excel**: Esportazione dati con formattazione avanzata

## 🚀 Avvio Rapido

1. Clona la repository
2. Apri `index.html` nel browser
3. Accedi con le credenziali di default

## 👤 Accessi

- **Amministratore**: Username: `Tommaso`, Password: `Tommy123`
- **Cliente**: Accesso guest senza credenziali

## 🔧 Configurazione

### Sincronizzazione GitHub Gist

Il sistema supporta sincronizzazione tramite GitHub Gist per l'utilizzo su più dispositivi:

1. Crea un token GitHub su Settings > Developer settings > Personal access tokens
2. Crea un nuovo Gist su gist.github.com
3. Inserisci token e Gist ID nel sistema
4. I dati verranno sincronizzati automaticamente

### Sistema di Sicurezza

- Password di default: `Tommy123`
- Protezione prezzi di acquisto per amministratori
- Auto-riattivazione sicurezza dopo 5 minuti

## 📱 Compatibilità

- Browser moderni (Chrome, Firefox, Safari, Edge)
- Responsive design per mobile e desktop
- Funzionamento offline con localStorage

## 🛠️ Tecnologie Utilizzate

- HTML5, CSS3, JavaScript ES6+
- SheetJS per export Excel
- GitHub API per sincronizzazione
- LocalStorage per persistenza dati

## 📋 Struttura del Progetto

```
tommy-wine-management/
├── index.html          # Applicazione principale
├── README.md           # Documentazione
├── CHANGELOG.md        # Log modifiche
├── LICENSE             # Licenza MIT
└── docs/              # Documentazione aggiuntiva
    ├── setup.md        # Istruzioni setup
    └── features.md     # Descrizione funzionalità
```

## 🔄 Funzionalità di Sincronizzazione

- Salvataggio automatico ogni 30 secondi
- Sincronizzazione tra dispositivi tramite GitHub Gist
- Fallback a localStorage in caso di errore
- Indicatori di stato sincronizzazione

## 🎨 Interfaccia Utente

- Design moderno e responsive
- Sistema di tab per navigazione
- Filtri avanzati per prodotti e vini
- Modal per configurazioni
- Notifiche in tempo reale

## 📊 Export e Import

- Export Excel con formattazione professionale
- Import da file Excel
- Stampa listino vini personalizzato
- Righe di intestazione fisse
- Formattazione automatica prezzi

## 🔒 Sicurezza

- Sistema di login con ruoli
- Censura prezzi di acquisto
- Password configurabile
- Timeout automatico sicurezza

## 📈 Roadmap

- [ ] Dashboard con statistiche
- [ ] Backup automatico
- [ ] Notifiche push
- [ ] API REST
- [ ] App mobile

## 🤝 Contributi

Le pull request sono benvenute. Per modifiche importanti, apri prima una issue per discutere cosa vorresti cambiare.

## 📄 Licenza

Questo progetto è sotto licenza MIT. Vedi il file `LICENSE` per i dettagli.

## 👨‍💻 Sviluppatore

Sviluppato per la gestione del bar e cantina "Privilege Cafè&Wine".

---

**🍷 Gestione Tommy** - Sistema professionale per la gestione di bar e cantine "Privilege Cafè&Wine" 