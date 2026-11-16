---
{"dg-publish":true,"permalink":"/bitcoin/spendere-bitcoin-ogni-giorno-dal-wallet-al-mercatino/","title":"🛒 Spendere bitcoin ogni giorno: dal wallet al mercatino","tags":["spendere-sats","lightning","barattolo","phoenix","economia-circolare","p2p"],"dg-note-properties":{"title":"🛒 Spendere bitcoin ogni giorno: dal wallet al mercatino","tags":["spendere-sats","lightning","barattolo","phoenix","economia-circolare","p2p"]}}
---

# 🛒 Spendere bitcoin ogni giorno: dal wallet al mercatino

Spendere bitcoin vuol dire usarli per comprare qualcosa da una persona, senza banca in mezzo. Non serve un piano complesso: servono una cifra piccola, un wallet Lightning e un posto dove spenderli.

Nel giardino ho già scritto [perché usare bitcoin conta](https://ortix.vercel.app/bitcoin/filosofia/bitcoin-non-e-una-spa/) e [come organizzare i fondi per viverci](https://ortix.vercel.app/bitcoin/guide-e-consigli/vivere-in-bitcoin/). Qui faccio una cosa sola: ti porto dal wallet vuoto al primo acquisto. Un percorso, nessuna scelta in più del necessario.

## 🤔 Perché partire da un acquisto

Chi compra bitcoin e li lascia fermi impara a custodire, ma non impara a usare. E un bitcoin che non circola è [una quota di SPA](https://ortix.vercel.app/bitcoin/filosofia/bitcoin-non-e-una-spa/): resta nel portafoglio, il potere resta dov'era.

Il primo acquisto ti insegna in dieci minuti cose che nessuna guida trasmette davvero:

- cos'è una fattura Lightning e perché scade;
- quanto costa davvero un pagamento;
- che dall'altra parte c'è una persona, non un circuito di carte.

Il posto più semplice per farlo è [Barattolo](https://barattolo.store), il mercatino in bitcoin creato da Alan, il mio giardiniere. Ci si compra e ci si vende in sats, tra persone.

## 🧭 Il percorso in 5 passi

### 1. Scegli una cifra piccola 💶

Decidi una somma che sei disposto a perdere mentre impari: **20-30 euro** vanno bene. Non scendere troppo: la prima ricezione su Lightning ha un costo di apertura del canale che pesa di più su cifre minuscole.

Regola semplice: è una cifra di studio, non un risparmio.

### 2. Installa un wallet Lightning self-custodial ⚡

Il percorso che propongo usa [Phoenix](https://ortix.vercel.app/bitcoin/lightning-network/phoenix/): è self-custodial, quindi le chiavi sono tue, e gestisce i canali in automatico. È il secondo gradino della [scala della sovranità su Lightning](https://ortix.vercel.app/bitcoin/lightning-network/00-come-essere-sovrano-su-ln-step-by-step/).

1. Installa Phoenix sullo smartphone.
2. Crea un nuovo wallet.
3. 🔑 Scrivi le 12 parole della seed phrase **su carta**, non in foto, non nelle note del telefono.
4. Verifica di averle copiate bene prima di ricevere un solo sat.

Perché non un wallet custodial? Si può, ed è il primo gradino della scala. Ma se impari a spendere senza tenere le chiavi, impari metà della lezione. Not your keys, not your coins.

### 3. Ricevi i primi sats 📥

Qui c'è il punto più delicato: come ottenere bitcoin senza consegnare i documenti a un exchange. Le strade P2P, senza KYC, sono quelle che trovi in [Bitcoin Dove iniziare](https://ortix.vercel.app/bitcoin/bitcoin-dove-iniziare/) e nella nota sul [P2P](https://ortix.vercel.app/bitcoin/p2-p/p2-p/): PeachBitcoin, Vexl, HodlHodl, Robosats, Bisq.

C'è anche una via più umana:

- fatti pagare in sats da un amico bitcoiner per un piccolo favore o un oggetto;
- vendi tu qualcosa su Barattolo e incassi direttamente in sats.

In Phoenix tocca **Ricevi**, genera la fattura Lightning e falla scansionare a chi ti paga. Dopo l'incasso controlla il saldo: vedrai già l'effetto delle commissioni di apertura.

### 4. Fai il primo acquisto su Barattolo 🛒

1. Apri [barattolo.store](https://barattolo.store) e scegli qualcosa di piccolo, coerente con il tuo saldo.
2. Leggi bene l'annuncio e, se serve, scrivi al venditore.
3. Al momento del pagamento segui il flusso indicato nelle [guide di Barattolo](https://www.barattolo.online): sono aggiornate e spiegano i passaggi esatti.
4. Quando ti viene mostrata la richiesta di pagamento, scansionala con Phoenix.
5. ✅ Prima di confermare controlla **importo e commissione** sullo schermo del wallet.
6. Conferma. Il pagamento Lightning arriva in pochi secondi.

Fatto. Hai appena pagato una persona senza chiedere il permesso a nessuno.

### 5. Chiudi il cerchio 🔄

Un acquisto è un esperimento. Un'abitudine nasce quando i sats tornano indietro:

- metti in vendita su Barattolo un oggetto che non usi più;
- incassa in sats sullo stesso wallet;
- spendi di nuovo.

È così che si forma un'economia circolare: piccola, locale, tra persone. Un seme piantato in un vaso, prima di pensare al campo.

## 📋 Riepilogo in una tabella

| Passo | Strumento | Cosa impari |
|---|---|---|
| Cifra | 20-30 € | Il costo reale di imparare |
| Wallet | Phoenix | Seed phrase e canali |
| Ricezione | P2P o amici | Ottenere sats senza KYC |
| Acquisto | Barattolo | Pagare una persona in sats |
| Cerchio | Vendere su Barattolo | Incassare e rispendere |

## ⚠️ Limiti e rischi

- **Commissioni**: Phoenix è comodo e la comodità si paga, con il costo di apertura del canale e una fee sulle transazioni. Su cifre piccole si nota. Quando ti serve di più, sali di gradino verso Blixt o Zeus, come spiego nella [guida step-by-step](https://ortix.vercel.app/bitcoin/lightning-network/00-come-essere-sovrano-su-ln-step-by-step/).
- **Seed persa = sats persi**: se perdi il telefono e non hai le 12 parole, nessuno può aiutarti. È il prezzo della self-custody.
- **Lightning non è una cassaforte**: tieni sul wallet Lightning solo la cifra per le spese. Il resto va sui livelli più bassi della [piramide dei fondi](https://ortix.vercel.app/bitcoin/guide-e-consigli/come-scegliere-il-wallet-giusto-flow-chart/).
- **P2P vuol dire persone**: valuta reputazione e recensioni di chi ti vende sats, e usa le piattaforme con escrow o depositi quando non conosci la controparte.
- **Un mercatino non è un negozio con call center**: controlla l'annuncio, fai domande prima di pagare, tieni traccia degli accordi.

Non è un consiglio finanziario: è un percorso per imparare con le mani.

## 🌱 Dove porta questo primo passo

Il primo acquisto non cambia il mondo. Cambia te: smetti di pensare a bitcoin come a un numero da guardare e inizi a usarlo come moneta. Da qui le strade sono due, e si possono fare insieme:

- organizzare i fondi per [vivere in Bitcoin](https://ortix.vercel.app/bitcoin/guide-e-consigli/vivere-in-bitcoin/), con il wallet Lightning ricaricato da un [hot wallet](https://ortix.vercel.app/bitcoin/definizioni/blockchain/hot-wallet/);
- salire la scala della sovranità fino a un nodo tuo.

Pagare in sats è un atto politico piccolo e ripetibile. La libertà esiste solo quando viene esercitata: inizia con 20 euro e un oggetto su [Barattolo](https://barattolo.store).
