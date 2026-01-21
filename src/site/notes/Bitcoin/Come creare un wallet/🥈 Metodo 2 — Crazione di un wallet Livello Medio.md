---
{"dg-publish":true,"permalink":"/bitcoin/come-creare-un-wallet/metodo-2-crazione-di-un-wallet-livello-medio/","title":"🥈 Metodo 2 — Crazione di un wallet Livello Medio","tags":["bitcoin","wallet","onchain","seed","entropia","sicurezza","autonomia"]}
---


# 🥈 Metodo 2 — Crazione di un wallet Livello Medio
## Seed generata dal wallet + passphrase umana (25ª parola)

Questo metodo è **il vero punto di svolta** tra:
- “conservo una seed”
- e **capisco cosa sto proteggendo**

Qui Bitcoin smette di essere solo matematica  
e diventa **responsabilità umana**.

---

## 🔑 L'Architettura della Passphrase

La "25ª parola" non è un semplice termine aggiuntivo della lista BIP39, ma un'estensione tecnica che trasforma la radice del wallet.

La Formula Fondamentale:

$$Wallet = Seed + Passphrase$$

- **Seed (senza passphrase):** Genera il Wallet A (Default).
    
- **Seed + Passphrase "X":** Genera il Wallet B.
    
- **Seed + Passphrase "Y":** Genera il Wallet C.

---

## 🛠️ Protocollo Operativo

### 1. Generazione e Importazione (Solo Blue Wallet)

Utilizza **esclusivamente [[Bitcoin/Wallet/Software Wallet/🔵 BlueWallet\|🔵 BlueWallet]]**.

**Creazione:**
Quando crei un nuovo wallet, abilita l'opzione "Passphrase" nelle impostazioni avanzate. La passphrase può essere una frase complessa, includere spazi e simboli (es. `Oltre la Luna 2026!`).

**Importazione:**
Quando devi importare un wallet con passphrase:
1. Clicca su "Aggiungi Wallet" -> "Importa".
2. Clicca sui **3 puntini in alto** a destra.
3. Seleziona "Passphrase" per abilitare il campo aggiuntivo.
4. Inserisci la Seed + la Passphrase.

> [!NOTE]
> Devi ripetere questa procedura (aggiungere la passphrase dai 3 puntini) ogni volta che vuoi importare un wallet diverso generato con lo stesso Seed ma una Passphrase differente.

### 2. La Strategia della Separazione Fisica (Regola d'Oro)

Il vantaggio di questo metodo risiede nella frammentazione del rischio:

- **Seed Phrase:** Custodita su supporto fisico (acciaio o carta) in un Luogo A.
    
- **Passphrase:** Memorizzata o custodita in un Luogo B.
    

> [!IMPORTANT] Se un malintenzionato trova solo la Seed, troverà un wallet vuoto (o un "wallet civetta"). Senza la passphrase, i fondi principali sono inaccessibili.

Esempi:
- `il mio primo nodo bitcoin`
- `Satoshi>Bancomat`
- `mare vento 1991 libertà`

⚠️ Ogni singolo carattere conta  
⚠️ Spazi inclusi

---

### 3️⃣ Scrivi separatamente (regola d’oro)

❌ Mai fare questo:
- seed + passphrase nello stesso posto

✅ Corretto:
- **Seed** → supporto fisico principale
- **Passphrase** → altrove, per esempio:
  - memoria
  - luogo fisico diverso

📌 Chi trova **solo la seed**  
👉 **non trova il wallet**

---

## 🪤 Wallet civetta (plausible deniability)

Puoi gestire la stessa Seed per scopi diversi:

- **Wallet Civetta (Senza Passphrase):** Contiene pochi fondi per uso quotidiano o per distrarre un eventuale aggressore.
- **Wallet "Vault" (Con Passphrase):** Il vero deposito, invisibile e non rintracciabile sulla blockchain come collegato al primo.
- **Wallet Secondario (Con Passphrase):** Possibilità di creare ulteriori wallet a partire dalla stessa passphrase

---

## ⚠️ Analisi dei Rischi

- 🔴 **Perdita Totale:** Se dimentichi la passphrase, la seed da sola è inutile. I fondi sono persi per sempre.
- 🔴 **Errore di Trascrizione:** Anche un singolo spazio o una maiuscola errata generano un wallet completamente diverso e vuoto. 
- 🔴 **Eccesso di Confidenza:** Scrivere seed e passphrase nello stesso luogo annulla ogni beneficio di sicurezza.

---
### 🔁 Una seed, molti wallet

Con questo metodo devi interiorizzare una cosa fondamentale:

> **Una singola seed può generare infiniti wallet**

Ogni volta che usi:
- la **stessa seed**
- con una **passphrase diversa**
- o **senza passphrase**

Blue Wallet crea **un wallet completamente distinto**.

Esempio concettuale:

- Seed + *(nessuna passphrase)* → Wallet 1  
- Seed + `ciao` → Wallet 2  
- Seed + `Ciao` → Wallet 3  
- Seed + `ciao ` → Wallet 4  
- Seed + `ciao ciao` → Wallet 5  

---

## 🧪 Best practice consigliate

✔ Usa una passphrase:
- non ovvia
- significativa per te
- ripetibile senza ambiguità

✔ Fai sempre un **test di ripristino**

✔ Tratta la passphrase come:
- una chiave mentale
- non come una password web

---

