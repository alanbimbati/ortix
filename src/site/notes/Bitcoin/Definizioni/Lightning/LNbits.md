---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/lightning/l-nbits/","title":"🔌 LNbits: la suite dei servizi Lightning","tags":["Bitcoin","Lightning","Definizione","Software","MultiUser"],"dg-note-properties":{"title":"🔌 LNbits: la suite dei servizi Lightning","tags":["Bitcoin","Lightning","Definizione","Software","MultiUser"],"aliases":["LNbits","LNbits suite"]}}
---


# 🔌 LNbits: la suite dei servizi Lightning

🧱 **LNbits** è un sistema di wallet e account multi-utente basato su [[Bitcoin/Lightning Network/⚡ Lightning Network\|Lightning Network]], che gira sopra una qualsiasi sorgente di finanziamento (come [[Bitcoin/Definizioni/Lightning/LND\|LND]], Core Lightning o altri nodi / wallet).

Può essere pensato come il "WordPress" di Lightning: una piattaforma modulare che permette di creare conti isolati per vari utenti ed estendere le funzionalità del proprio nodo tramite una vasta libreria di estensioni.

⚠️ **Chi usa un sub-wallet è in custodia.** I wallet creati su LNbits non hanno chiavi proprie: i sats stanno nel nodo dell'amministratore. Per l'utente LNbits è un servizio custodial, come [Wallet of Satoshi](https://ortix.vercel.app/bitcoin/wallet/software-wallet/wallet-of-satoshi/). La differenza è che il custode è una persona che conosci. Se l'amministratore spegne il server, perde il nodo o blocca un account, l'utente non ha modo di recuperare i fondi da solo. Va bene per piccole cifre e dove la fiducia è reale (famiglia, associazione, negozio). Il patrimonio resta in self-custody, alla base della [piramide dei fondi](https://ortix.vercel.app/bitcoin/guide-e-consigli/come-scegliere-il-wallet-giusto-flow-chart/).

---

## 🏗️ A Cosa Serve?

Con LNbits puoi:
* **Creare portafogli diversi**: Utile in scenari familiari, scolastici o industriali, dove una sola persona gestisce il nodo LND ma fornisce piccoli wallet indipendenti a collaboratori o amici.
* **Installare estensioni**: LNbits ha un catalogo di plugin come POS (registratori di cassa per esercenti), Tip Cards (carte regalo Lightning), Paywalls (per sbloccare articoli o contenuti tramite micro-pagamenti), e pay-links.
* **Delegare l'accesso**: Consente a wallet come [[Bitcoin/Lightning Network/Zeus\|Zeus]] di connettersi a specifiche estensioni (es. LNbits LNDHub) per transare da cellulare senza esporre le restanti finanze del nodo primario.

---

## 🎯 Il Framework di Responsabilità

1. **Chi decide?** L'amministratore del server (che installa LNbits sul proprio [[Bitcoin/Definizioni/Blockchain/Full Node\|Full Node]]) decide a quali utenti dare accesso alla piattaforma, quali estensioni attivare e in che misura limitare le capacità dei vari wallet dipendenti.
2. **Quali incentivi ha?** Ha l'incentivo a fornire un'interfaccia ricca di strumenti e automazioni senza forzare gli utenti secondari a gestire un intero nodo.
3. **Chi è responsabile?** L'amministratore del nodo di finanziamento sottostante è responsabile dell'uptime e della liquidità on-chain/off-chain. Gli utenti dei sub-wallet di LNbits si fidano dell'amministratore (relazione [[Bitcoin/Definizioni/Lightning/Custodial\|Custodial]] interna).

---

🔗 _Vedi anche: [[Bitcoin/Lightning Network/00 - Come Essere Sovrano su LN (Step-by-Step)\|00 - Come Essere Sovrano su LN (Step-by-Step)]], [[Bitcoin/Lightning Network/Zeus\|Zeus]], [[Bitcoin/Definizioni/Lightning/LND\|LND]], [[Bitcoin/Definizioni/Lightning/Routing\|Routing]], [[Bitcoin/Lightning Network/⚡ Lightning Network\|⚡ Lightning Network]]_
