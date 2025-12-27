# 🎬 TV Channels Manager

Un'applicazione web completa e interattiva per gestire i tuoi canali TV preferiti. Organizza, categorizza e accedi rapidamente ai tuoi canali televisivi preferiti!

## ✨ Caratteristiche Principali

### 🎯 Gestione Completa
- **Aggiungi Canali**: Inserisci nome, URL e immagine del logo
- **Organizza in Gruppi**: Crea categorie personalizzate (es. "Sport", "News", "Intrattenimento")
- **Modifica Canali**: Clicca l'icona ✏️ per modificare nome, URL, immagine o gruppo
- **Modifica Gruppi**: Rinomina i tuoi gruppi con un click
- **Riordina Drag & Drop**: Trascina i canali per riordinarli o spostarli tra gruppi
- **Elimina Facilmente**: Rimuovi canali o interi gruppi con l'icona 🗑️
- **Interfaccia Intuitiva**: Design moderno e user-friendly

### 💾 Salvataggio Automatico
- Tutti i dati sono salvati automaticamente nel browser (localStorage)
- Nessuna registrazione o server richiesto
- I tuoi dati rimangono privati sul tuo dispositivo

### 📤 Import/Export
- **Esporta**: Salva tutti i tuoi canali in un file JSON
- **Importa**: Ripristina i dati da un backup o condividi le tue configurazioni
- File di esempio incluso (`sample-data.json`)

### 🎨 Design Responsive
- Ottimizzato per desktop, tablet e smartphone
- Tema scuro moderno
- Animazioni fluide e interattive
- Immagini uniformi (600x600px)

## 🚀 Come Usare

### Primo Avvio

1. **Apri** `tv-manager.html` nel tuo browser
2. Vedrai due gruppi predefiniti: "Canali Nazionali" e "Canali Internazionali"

### Aggiungere un Canale

1. Compila il form nel pannello amministrazione:
   - **Nome Canale**: es. "RAI News 24"
   - **URL Canale**: link alla diretta streaming
   - **URL Immagine**: link al logo del canale (600x600px consigliato)
   - **Gruppo**: seleziona da menu a tendina

2. Clicca **"Aggiungi Canale"**
3. Il canale apparirà immediatamente nella categoria scelta

### Creare un Nuovo Gruppo

1. Clicca **"Nuovo Gruppo"** nel pannello amministrazione
2. Inserisci il nome del gruppo (es. "Canali Sport", "Documentari")
3. Clicca **"Crea"**
4. Il nuovo gruppo sarà disponibile nel menu a tendina

### Modificare un Canale

1. Passa il mouse sulla card del canale
2. Clicca l'icona **✏️** (matita blu) in alto a destra
3. Modifica i dati nel modal che si apre
4. Clicca **"Salva Modifiche"**

### Modificare un Gruppo

1. Trova l'header del gruppo
2. Clicca **"✏️ Modifica"** accanto al nome del gruppo
3. Inserisci il nuovo nome
4. Clicca **"Salva Modifiche"**
   - Tutti i canali del gruppo vengono aggiornati automaticamente

### Riordinare i Canali (Drag & Drop)

1. **Clicca e tieni premuto** su una card di canale
2. **Trascina** la card nella posizione desiderata
3. **Rilascia** per posizionare il canale
4. Puoi anche **trascinare tra gruppi diversi** per spostare un canale
5. L'ordine viene salvato automaticamente

### Eliminare Elementi

- **Canale**: Clicca l'icona **🗑️** (cestino rosso) in alto a destra della card
- **Gruppo**: Clicca **"🗑️ Elimina"** nell'header del gruppo
  - ⚠️ Attenzione: eliminerà anche tutti i canali nel gruppo

### Backup e Ripristino

**Esportare i Dati:**
1. Clicca **"Esporta Dati"**
2. Verrà scaricato un file JSON con tutti i tuoi canali

**Importare i Dati:**
1. Clicca **"Importa Dati"**
2. Seleziona un file JSON precedentemente esportato
3. Conferma la sostituzione dei dati attuali

## 📁 File Inclusi

```
tv-channels-manager/
├── tv-manager.html      # Applicazione principale (HTML + CSS + JS)
├── sample-data.json     # Dati di esempio con canali pre-configurati
└── README.md           # Questa documentazione
```

## 🔧 Utilizzo del File di Esempio

Per iniziare con alcuni canali già configurati:

1. Apri `tv-manager.html`
2. Clicca **"Importa Dati"**
3. Seleziona `sample-data.json`
4. Conferma l'importazione

Il file include:
- 6 Canali Nazionali (RAI News, Sky TG24, TGCom24, Rainews.it, La7, Rai 1)
- 5 Canali Internazionali (BBC, CNN, France 24, DW News, Al Jazeera)

## 💻 Tecnologie

- **HTML5**: Struttura semantica moderna
- **CSS3**: Grid Layout, Flexbox, animazioni, gradienti
- **JavaScript (Vanilla)**: Nessuna dipendenza esterna
- **localStorage API**: Persistenza dei dati nel browser

## 🌐 Compatibilità Browser

- ✅ Chrome/Edge (versioni recenti)
- ✅ Firefox (versioni recenti)
- ✅ Safari (versioni recenti)
- ✅ Opera (versioni recenti)

Richiede supporto per:
- localStorage
- ES6+ JavaScript
- CSS Grid e Flexbox

## 📱 Responsive Design

L'applicazione si adatta automaticamente a:
- 🖥️ **Desktop**: Layout a griglia multipla
- 📱 **Tablet**: Layout a 2-3 colonne
- 📲 **Mobile**: Layout a colonna singola

## 🎨 Personalizzazione

### Modificare i Colori

Cerca nel CSS (sezione `<style>`) le seguenti variabili:

```css
/* Colore primario (viola) */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Sfondo principale */
background-color: #1a1a1a;

/* Card background */
background: #2a2a2a;
```

### Modificare le Dimensioni delle Immagini

Nel CSS, cerca `.tv-image`:

```css
.tv-image {
    height: 300px;  /* Modifica questa altezza */
}
```

## 🔐 Privacy e Sicurezza

- ✅ Tutti i dati sono salvati SOLO sul tuo browser
- ✅ Nessun dato inviato a server esterni
- ✅ Nessun tracking o analytics
- ✅ Funziona completamente offline (dopo il primo caricamento)

## 🐛 Risoluzione Problemi

### I dati non vengono salvati
- Verifica che il browser abbia i cookie/localStorage abilitati
- Controlla di non essere in modalità navigazione privata

### Le immagini non si caricano
- Verifica che l'URL dell'immagine sia corretto
- Alcuni siti potrebbero bloccare l'hotlinking delle immagini
- Usa servizi di hosting immagini come Imgur o carica su GitHub

### Il backup non si importa
- Verifica che il file sia in formato JSON valido
- Controlla che contenga le chiavi `channels` e `groups`

## 📝 Suggerimenti per le Immagini

**Dove trovare loghi dei canali:**
- Siti ufficiali dei canali TV
- [Wikimedia Commons](https://commons.wikimedia.org/)
- [Logos-world.net](https://logos-world.net/)
- Ricerca Google Immagini (filtra per dimensione grande e diritti d'uso)

**Dimensioni consigliate:**
- Minimo: 512x512px
- Consigliato: 600x600px
- Massimo: 1024x1024px
- Formato: PNG con sfondo trasparente (ideale)

## 🎯 Esempi di Gruppi

Alcuni suggerimenti per organizzare i tuoi canali:

- 📺 **Per Tipo**: News, Sport, Intrattenimento, Documentari, Cinema
- 🌍 **Per Regione**: Nazionali, Europei, Americani, Asiatici
- 🏷️ **Per Tema**: Politica, Tecnologia, Cultura, Musica
- ⭐ **Per Frequenza**: Preferiti, Occasionali, Archivio

## 📚 Esempi di Utilizzo

### Esempio 1: Aggiungere un Canale Sportivo
```
Nome: ESPN
URL: https://www.espn.com/watch/
Immagine: https://example.com/espn-logo.png
Gruppo: Sport
```

### Esempio 2: Creare Gruppo Tematico
```
Nome Gruppo: Canali Musicali
Canali: MTV, VH1, Music Box, Trace Urban
```

## 🚀 Pubblicazione su GitHub Pages

1. Crea un repository su GitHub
2. Carica i file (tv-manager.html, sample-data.json, README.md)
3. Vai su Settings → Pages
4. Seleziona "main" branch → "root"
5. La tua app sarà su: `https://[username].github.io/[repo-name]/tv-manager.html`

## 🔄 Aggiornamenti Futuri

Possibili miglioramenti:
- [x] Riordinamento personalizzato (drag & drop) ✅
- [x] Modifica canali ✅
- [x] Modifica gruppi ✅
- [ ] Ricerca/filtro canali
- [ ] Temi colore multipli
- [ ] Supporto per sottogruppi
- [ ] Preview immagine prima del caricamento
- [ ] Statistiche di utilizzo
- [ ] Modalità griglia/lista
- [ ] Esportazione in HTML statico

## 📄 Licenza

Questo progetto è rilasciato sotto licenza **CC-0** (pubblico dominio).
Sei libero di:
- ✅ Usare per scopi personali o commerciali
- ✅ Modificare e personalizzare
- ✅ Distribuire e condividere
- ✅ Includere in altri progetti

## 👨‍💻 Autore

Creato con ❤️ da **Mauro**

## 🙏 Crediti

- Design ispirato da moderne UI/UX guidelines
- Icone emoji native del sistema
- Loghi dei canali TV © rispettivi proprietari

---

**Buon utilizzo! 🎉**

Per domande o suggerimenti, apri una Issue su GitHub.
