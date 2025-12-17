---
{"dg-publish":true,"permalink":"/bitcoin/wallet/hardware-wallet/krux/","title":"🟠 Krux: SeedSigner open source per tutti","tags":["Bitcoin","Wallet","Hardware","DIY","OpenSource","Airgap","BitcoinOnly","Stateless"]}
---


# 🟠 Krux: SeedSigner open source per tutti

🛠️ **Krux è il cugino accessibile di SeedSigner.**  
Stesso concetto (DIY, stateless, airgapped) ma con hardware più economico e semplice da trovare.

---

## 🔐 Cos'è Krux?

Krux è un **[[Bitcoin/Wallet/Hardware Wallet\|hardware wallet]]** completamente **DIY** (Do It Yourself) e **stateless**, proprio come [[Bitcoin/Wallet/✍️ SeedSigner\|✍️ SeedSigner]].

**Differenze principali:**
- **Hardware**: dispositivi **M5StickV** o **Amigo** (più economici e disponibili)
- **Software**: firmware Krux (fork migliorato di SeedSigner)
- **Costo**: ~30-60€ totale per il kit

🟠 È il modo **più economico** per avere un signing device airgapped Bitcoin-only.

---

## 📱 Caratteristiche

### ✅ Punti di Forza

- **Completamente stateless** → non conserva mai la seed
- **DIY e open source al 100%** → massima trasparenza
- **Bitcoin-only** → nessuna distrazione
- **Airgapped** → solo QR code
- **Economico** → ~30-60€ (vs ~150€ di SeedSigner assemblato)
- **Hardware più reperibile** → M5StickV facilmente disponibile online
- **Fotocamera** → per scansionare PSBT e wallet import
- **Display** → piccolo ma sufficiente
- **Sempre verificabile** → ricompili e verifichi tu stesso

### ⚠️ Limiti

- **Devi assemblarlo** → non plug-and-play
- **Display piccolo** → M5StickV ha schermo minuscolo
- **UX spartana** → funzionale ma non elegante
- **Nessun supporto ufficiale** → community-driven
- **Devi inserire seed ogni volta** → stateless = meno comodo

---

## 🛠️ Come Funziona (Stateless)

Krux **non conserva mai la tua seed in memoria.**

**Workflow:**
1. Accendi il device
2. Inserisci la tua seed (manualmente o via QR)
3. Firmi la transazione
4. Spegni il device → **seed dimenticata per sempre**

📡 Prossima volta che lo accendi, devi **re-inserire la seed.**

**Perché è sicuro?**
- Se qualcuno ruba il device, **non trova nulla**
- Nessun attacco fisico può estrarre chiavi (non esistono in memoria)
- Massima sicurezza **se custodisci la seed esternamente** ([[Bitcoin/Wallet/🪨 Steelwallet\|🪨 Steelwallet]])

---

## 🆚 Krux vs SeedSigner

| Feature | SeedSigner | Krux |
|---------|-----------|------|
| **Hardware** | Raspberry Pi Zero | M5StickV / Amigo |
| **Display** | 320x240 (buono) | 135x240 (piccolo) |
| **Prezzo** | ~80-150€ | ~30-60€ |
| **Disponibilità** | Hardware scarso | Facile da trovare |
| **Software** | SeedSigner | Krux (fork) |
| **Community** | Più grande | Emergente |

🟠 **Krux è SeedSigner economico con hardware più disponibile.**

---

## 🧠 Funzionalità

- Firma [[Bitcoin/Wallet/✍️ PSBT\|✍️ PSBT]] via QR code
- Supporta [[Bitcoin/Wallet/🔐 Multisig\|🔐 Multisig]]
- Generazione seed con **dadi** (massima entropia verificabile)
- Import/export seed via QR code
- Compatibile con [[Bitcoin/Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]], [[Bitcoin/Wallet/⚡ Electrum\|⚡ Electrum]], [[Bitcoin/Wallet/🔵 BlueWallet\|🔵 BlueWallet]]
- Verifica indirizzi di ricezione
- Firmware aggiornabile e compilabile

🛠️ È un **signing device puro**: non gestisce UTXO, non si connette a nodi.  
Serve solo a **firmare transazioni in modo sicuro.**

---

## 🎯 Per chi è adatto?

✅ **Buono per:**
- **Smanettoni** che vogliono costruire il proprio wallet
- Chi cerca **massima trasparenza** (DIY + open source)
- Chi vuole **stateless** per sicurezza massima
- **Budget limitato** (~30-60€)
- Bitcoin-only purists
- Chi apprezza il concetto di **"nothing to extract"**

❌ **Non ideale per:**
- Principianti che vogliono plug-and-play
- Chi vuole display grande e UX moderna
- Chi non vuole inserire seed ogni volta
- Chi cerca supporto ufficiale e garanzia

---

## 🔥 Opinione

Krux è **l'hardware wallet più cypherpunk che esista.**

🟠 **Massima trasparenza**: tu costruisci, verifichi, compili.  
**Massima sicurezza**: stateless, airgapped, Bitcoin-only.  
**Minimo costo**: ~30-60€.

⚠️ **MA**: UX spartana, display piccolo, setup manuale.

💡 Se sei **tecnico, paranoico, e vuoi il miglior rapporto sicurezza/prezzo**, Krux è **imbattibile.**

🛠️ Se vuoi comodità, prendi [[Bitcoin/Wallet/Hardware Wallet/🟢 Jade\|🟢 Jade]], [[Bitcoin/Wallet/Hardware Wallet/🔷 BitBox02\|🔷 BitBox02]] o [[Bitcoin/Wallet/Hardware Wallet/🔴 Trezor\|🔴 Trezor]].

---

## ✅ Conclusione

Krux è **per chi vuole costruire la propria sovranità, letteralmente.**

🎯 Usalo se:
- Sei smanettone e apprezzi DIY
- Vuoi massima trasparenza e sicurezza
- Budget molto limitato
- Sei Bitcoin-only purista
- Vuoi stateless per "nothing to extract"

🚫 Considera alternative se:
- Vuoi plug-and-play
- Cerchi display grande e UX moderna
- Non vuoi gestire seed manualmente
- Vuoi supporto ufficiale

🟠 **Krux: massima sicurezza, minimo costo, massima libertà.**

---

🔗 _Sito ufficiale: [selfcustody.github.io/krux](https://selfcustody.github.io/krux)_

📎 _Vedi anche: [[Bitcoin/Wallet/Hardware Wallet\|Hardware Wallet]], [[Bitcoin/Wallet/✍️ SeedSigner\|✍️ SeedSigner]], [[Bitcoin/Wallet/❄️ Coldcard\|❄️ Coldcard]], [[Bitcoin/Wallet/🔐 Self-custody\|🔐 Self-custody]], [[Bitcoin/Wallet/✍️ PSBT\|✍️ PSBT]], [[Bitcoin/Wallet/🧠 Seed Phrase\|🧠 Seed Phrase]]_
