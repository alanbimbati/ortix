---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/lightning/custodial/","title":"🌐 Custodial: delegare le chiavi","tags":["Bitcoin","Custody","Definizione","Lightning"],"dg-note-properties":{"title":"🌐 Custodial: delegare le chiavi","tags":["Bitcoin","Custody","Definizione","Lightning"],"aliases":["Custodiale","custodial","servizi custodial"]}}
---


# 🌐 Custodial: delegare le chiavi

🔑 Nel mondo di Bitcoin, un servizio o un wallet si definisce **Custodial** (custodiale) quando **affidi la gestione delle tue chiavi private a una terza parte**. 

In pratica, non sei tu a possedere la chiave crittografica che sblocca i fondi, ma l'azienda che fornisce l'applicazione.

---

## 🎯 Il Framework di Responsabilità

Per capire a fondo il modello custodial, applichiamo le tre domande chiave di Ortix:

1. **Chi decide?** L'azienda o il fornitore del servizio. Loro controllano il software, gli indirizzi on-chain e i canali Lightning.
2. **Quali incentivi ha?** Ha l'incentivo di rendere l'esperienza utente il più semplice e immediata possibile per attirare utenti, ma deve anche obbedire alle regolamentazioni governative (KYC/AML) per evitare la chiusura del servizio.
3. **Chi è responsabile?** In teoria l'azienda, ma in pratica **lo sei tu** se le cose vanno male. Se l'azienda fallisce o viene bloccata, i tuoi fondi spariscono.

---

## ⚖️ Vantaggi e Svantaggi

### ✅ Vantaggi
* **Configurazione zero**: Nessuna seed phrase da annotare, nessuna gestione tecnica dei canali.
* **Recupero facile**: Se perdi la password, puoi recuperare l'account tramite email o supporto clienti.
* **Costi di onboarding azzerati**: Spesso non paghi le fee on-chain per l'apertura manuale dei canali, poiché usi l'infrastruttura condivisa del provider.

### ❌ Svantaggi e Rischi
* **Rischio di controparte**: *"Not your keys, not your coins"*. Se l'azienda chiude o congela il tuo account, non hai vie legali o crittografiche per riprenderti i bitcoin.
* **Zero privacy**: Tutte le tue transazioni sono registrate sul database centralizzato dell'azienda.
* **Censura**: L'azienda può rivelare i tuoi dati o bloccarti i fondi se costretta dalle autorità.

---

## 🧭 Dove si colloca nel percorso?

Un wallet custodial come [[Bitcoin/Lightning Network/Wallet of Satoshi\|Wallet of Satoshi]] è un ottimo punto di partenza per testare la tecnologia con pochi euro. Ma per importi significativi, la sovranità impone il passaggio alla [[Bitcoin/Definizioni/Blockchain/🔐 Self-custody\|Self-Custody]].
