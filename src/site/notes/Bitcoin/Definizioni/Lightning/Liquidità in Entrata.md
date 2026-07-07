---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/lightning/liquidita-in-entrata/","title":"📥 Liquidità in Entrata: la capacità di ricevere","tags":["Bitcoin","Lightning","Definizione","Liquidità"],"dg-note-properties":{"title":"📥 Liquidità in Entrata: la capacità di ricevere","tags":["Bitcoin","Lightning","Definizione","Liquidità"],"aliases":["Liquidità in entrata","inbound liquidity","liquidità"]}}
---


# 📥 Liquidità in Entrata: la capacità di ricevere

⚡ In [[Bitcoin/Lightning Network/⚡ Lightning Network\|Lightning Network]], la **Liquidità in Entrata** (Inbound Liquidity) indica la quantità di satoshi che si trovano sull'altro lato di un [[Bitcoin/Definizioni/Lightning/Canale di Pagamento\|Canale di Pagamento]] e che, quindi, possono essere inviati verso di te.

Se non possiedi liquidità in entrata, **non puoi ricevere pagamenti**.

---

## 💡 La metafora della clessidra

Immagina un canale Lightning come una clessidra:
* All'inizio la sabbia (i satoshi) si trova tutta nella parte superiore (la tua parte del canale: **liquidità in uscita** o *outbound liquidity*). Puoi inviare fondi svuotando la tua metà.
* Ma se la parte inferiore (la parte del tuo peer) è completamente vuota, non c'è sabbia da far scendere verso di te. Non puoi ricevere finché non hai prima speso dei soldi, oppure finché qualcuno non ha aperto un canale immettendo fondi dalla sua parte.

---

## 🎯 Il Framework di Responsabilità

1. **Chi decide?** Chiunque apra un canale decide la direzione dei fondi iniziali. Se apri tu un canale, crei solo liquidità in uscita. Se lo apre un altro peer verso di te, ottieni liquidità in entrata.
2. **Quali incentivi ha?** Un utente ordinario ha l'incentivo di avere canali bilanciati per poter sia inviare che ricevere senza intoppi. Alcuni servizi offrono "Inbound Liquidity on demand" a pagamento per consentire la ricezione immediata.
3. **Chi è responsabile?** Tu sei responsabile di comprendere lo stato del tuo canale prima di richiedere un pagamento. Se usi wallet avanzati come [[Bitcoin/Lightning Network/Blixt\|Blixt]] o [[Bitcoin/Lightning Network/Zeus\|Zeus]], devi pianificare la liquidità o fare affidamento su meccanismi automatizzati come i canali LSP (Lightning Service Provider).

---

## 🚀 La soluzione di Blixt e dei wallet moderni

La "figata" di wallet come [[Bitcoin/Lightning Network/Blixt\|Blixt]] è che gestiscono la liquidità in entrata in modo semiautomatico. Se stai provando a ricevere sats e non hai abbastanza spazio sul canale, il wallet richiede a un nodo partner (LSP) di aprirti al volo un canale verso di te, prelevando una piccola fee per coprire il costo on-chain. In questo modo ricevi subito senza configurazioni tecniche complesse.

---

🔗 _Vedi anche: [[Bitcoin/Lightning Network/00 - Come Essere Sovrano su LN (Step-by-Step)\|00 - Come Essere Sovrano su LN (Step-by-Step)]], [[Bitcoin/Definizioni/Lightning/Canale di Pagamento\|Canale di Pagamento]], [[Bitcoin/Definizioni/Lightning/Routing\|Routing]], [[Bitcoin/Lightning Network/Blixt\|Blixt]], [[Bitcoin/Lightning Network/Zeus\|Zeus]]_
