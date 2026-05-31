---
{"dg-publish":true,"permalink":"/bitcoin/come-creare-un-wallet/metodo-3-crazione-di-un-wallet-livello-difficile/","title":"🥇 Metodo 3 — Crazione di un wallet Livello Difficile","tags":["bitcoin","wallet","onchain","seed","entropia","sicurezza","autonomia"],"dg-note-properties":{"title":"🥇 Metodo 3 — Crazione di un wallet Livello Difficile","tags":["bitcoin","wallet","onchain","seed","entropia","sicurezza","autonomia"],"status":"evergreen"}}
---


# 🥇 Metodo 3 — Crazione di un wallet Livello Difficile
## 🎲 Perché usare i dadi? (Massima Entropia)

Il vantaggio principale di questo metodo è la **Massima Entropia** e l'assenza di fiducia verso terzi.
Quando usi un software per generare le parole, ti stai fidando che il generatore di numeri casuali del computer sia davvero casuale e non compromesso.

Usando i dadi:
1. **Non ti fidi di nessun algoritmo:** La casualità è fisica, generata dalla gravità e dal movimento.
2. **Nessuna Backdoor:** Nessuno può aver programmato i dadi per uscire in una certa sequenza.
3. **Sovranità Totale:** Sei tu, fisicamente, a creare la tua chiave privata.

---

## 🛠️ Come fare (Procedura Semplificata)

Non serve essere matematici. **[[Bitcoin/Wallet/Software Wallet/🔵 BlueWallet\|🔵 BlueWallet]]** ha una funzione nascosta che ci permette di inserire l'entropia dei dadi direttamente, occupandosi lui dei calcoli complessi (checksum), ma senza generare la casualità al posto tuo.

### Strumenti
- **Generatore di casualità:**
  - **Dado a 6 facce (D6):** Il classico dado da gioco.
  - **Dado a 20 facce (D20):** Tipico di Dungeons & Dragons.
  - **Moneta:** Testa o Croce.
- **Blue Wallet** installato su un dispositivo offline (modalità aereo) per massima sicurezza.

> [!TIP] I Dadi Platonici (Grazie a Bubble per la dritta!)
> È fondamentale che il dado utilizzato sia un **Solido Platonico**, ovvero una figura geometrica con facce identiche e regolari, per garantire che ogni faccia abbia esattamente la stessa probabilità di uscire.
> Sia il **D6** (cubo) che il **D20** (icosaedro) sono solidi platonici, quindi perfetti per questo scopo.
>
> Il concetto rimane lo stesso per tutti gli strumenti: cambia solo il numero di lanci necessari per raggiungere l'entropia richiesta (una moneta ha meno "variabili" di un D20, quindi richiederà più lanci).

### Procedura Passo-Passo

1. **Apri Blue Wallet** e vai su "Aggiungi Wallet".
2. Seleziona **Bitcoin**.
3. Invece di cliccare "Crea", scorri in basso e clicca su **"Fornisci entropia"** (o "Provide Entropy").
4. Seleziona l'opzione **"Dice"** (Dadi).
5. **Lancia il dado** fisicamente.
6. Digita sul telefono il numero uscito (da 1 a 6).
7. **Ripeti** l'operazione fino a riempire la barra di progresso (servono circa 100 lanci per 24 parole).
8. Quando hai finito, Blue Wallet calcolerà automaticamente la **Seed Phrase** valida corrispondente ai tuoi lanci.

> [!TIP]
> Questo metodo unisce la sicurezza dell'entropia fisica con la comodità del software che fa i calcoli per te, eliminando il rischio di errore umano nel calcolo manuale.
    

---

## ⚖️ Analisi della Responsabilità

> [!WARNING]
> 
> In questo metodo, Bitcoin non ti protegge dai tuoi errori. Se sbagli il calcolo del checksum o la mappatura, potresti generare un wallet che non sarai in grado di ripristinare in futuro.

### Vantaggi

- **Inattaccabilità:** Nessun hacker può prevedere la tua chiave tramite vulnerabilità software.
    
- **Pieno Controllo:** Sei l'unico responsabile della genesi dei tuoi fondi.
    

### Svantaggi

- **Complessità Tecnica:** Richiede precisione matematica e tempo.
    
- **Errore Umano:** Il rischio di sbagliare la conversione o la scrittura è più alto rispetto ai metodi automatizzati.
    

---

## 📲 Importazione e Verifica (Solo Blue Wallet)

Una volta generata la seed con i dadi, devi importarla in un software per usarla. Utilizza **[[Bitcoin/Wallet/Software Wallet/🔵 BlueWallet\|🔵 BlueWallet]]**.

### Importazione
1. Apri Blue Wallet e clicca su "Aggiungi Wallet" -> "Importa".
2. Inserisci le 12 o 24 parole generate con i dadi.
3. **Se hai deciso di usare una Passphrase (consigliato):**
   - Clicca sui **3 puntini in alto** a destra nella schermata di importazione.
   - Seleziona "Passphrase" per abilitare il campo aggiuntivo.
   - Inserisci la Passphrase scelta.

> [!NOTE]
> Se usi una passphrase, ricorda che ogni combinazione diversa di Seed + Passphrase genera un wallet diverso. Per importare un altro wallet derivato dallo stesso seed ma con passphrase diversa, ripeti la procedura usando i 3 puntini.

### 🧪 Stress Test (Obbligatorio)
Prima di inviare fondi:
1. Importa il wallet come descritto sopra.
2. Annotati un indirizzo di ricezione o l'impronta del wallet.
3. **Cancella** il wallet dall'app.
4. **Ripristinalo** da zero usando solo i tuoi appunti (Seed + eventuale Passphrase).
5. Se l'indirizzo/impronta coincide, il backup è corretto.