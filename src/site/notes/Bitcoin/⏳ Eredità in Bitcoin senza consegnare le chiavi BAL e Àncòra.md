---
{"dg-publish":true,"permalink":"/bitcoin/eredita-bitcoin-senza-consegnare-le-chiavi-bal-ancora/","title":"⏳ Eredità in Bitcoin senza consegnare le chiavi: BAL e Àncòra","tags":["eredita","timelock","electrum","self-custody","utxo","privacy"],"dg-note-properties":{"title":"⏳ Eredità in Bitcoin senza consegnare le chiavi: BAL e Àncòra","tags":["eredita","timelock","electrum","self-custody","utxo","privacy"]}}
---

# ⏳ Eredità in Bitcoin senza consegnare le chiavi: BAL e Àncòra

Un'eredità a transazioni con scadenza è una transazione Bitcoin che firmi oggi, ma che la rete accetta solo dopo una certa data o una certa altezza di blocco. Se sei vivo, la rinnovi prima della scadenza. Se non ci sei più, parte verso gli eredi. Le chiavi restano sempre tue.

## 🌱 Da dove arriva questo seme

Il seme l'ha portato Manuelll-X: il **protocollo BAL** e il plugin **Àncòra** per [Electrum](https://ortix.vercel.app/bitcoin/wallet/software-wallet/electrum/) propongono un'eredità decentralizzata basata su transazioni a tempo.

La mia nota [Eredità in Bitcoin](https://ortix.vercel.app/bitcoin/eredita-in-bitcoin/) parla di seed su carta o metallo, cassaforti e lettere di istruzioni. Funziona, ma ha un punto debole: prima o poi qualcuno deve **trovare le chiavi**. Questa nota non sostituisce quella. La completa con un'altra strada.

⚠️ Qui spiego il meccanismo, non il manuale. Intervalli di rinnovo, compensi e formato dei dati di Àncòra e di BAL vanno verificati nella loro documentazione.

## 🧩 Il problema: le chiavi sono un'arma a doppio taglio

Con la [self-custody](https://ortix.vercel.app/bitcoin/definizioni/blockchain/self-custody/) la [seed phrase](https://ortix.vercel.app/bitcoin/definizioni/blockchain/seed-phrase/) è il patrimonio. Per l'eredità questo crea un dilemma:

- se consegni la seed oggi, chi la riceve può spendere **oggi**;
- se la nascondi troppo bene, sparisce **con te**;
- la [multisig](https://ortix.vercel.app/bitcoin/definizioni/blockchain/multisig/) distribuisce il rischio, ma richiede persone fidate che custodiscano chiavi e sappiano usarle.

Le transazioni a tempo tolgono di mezzo il passaggio più delicato. Agli eredi arriva una **transazione già firmata** che nessuno può usare prima del momento giusto, non la chiave.

## ⏳ L'idea: una lettera «da aprire dopo il…» che nessuno può aprire prima

Bitcoin permette di firmare una transazione con un **lucchetto temporale**: finché non si raggiunge un certo blocco o una certa data, i nodi la rifiutano come non valida. È una busta con scritto «da aprire dopo il 2030», con una differenza: qui non dipende dalla buona fede di chi la tiene, perché sono i nodi a rifiutarla.

Il flusso, a grandi linee:

1. **Scegli gli eredi**: ognuno ti fornisce un indirizzo del *proprio* wallet non custodial.
2. **Il wallet costruisce la transazione**: spende i tuoi [UTXO](https://ortix.vercel.app/bitcoin/definizioni/blockchain/utxo/) verso gli indirizzi degli eredi, con una scadenza futura.
3. **Firmi tu**: la firma avviene nel tuo wallet e le chiavi non escono.
4. **Consegni la transazione firmata** ai *will-executor*, uno o più.
5. **Finché ci sei, rinnovi**: prima della scadenza sposti i fondi o ne firmi una nuova con una data più lontana.
6. **Se non rinnovi**, alla scadenza l'executor trasmette la transazione e i sats arrivano agli eredi.

🔑 Il rinnovo funziona grazie al modello UTXO. Un output si spende **una sola volta**: se sposti anche solo uno degli UTXO usati nella vecchia transazione, quella diventa invalida per sempre e nessuno può più trasmetterla.

## 🤝 I will-executor: cosa possono fare e cosa vedono

Il will-executor è il «postino» della tua eredità: conserva la transazione firmata e la trasmette quando diventa valida. Usarne diversi e indipendenti rende il sistema **decentralizzato**: nessuno è indispensabile, basta che uno solo faccia il suo lavoro.

✅ **Non può:**
- cambiare destinatari o importi, perché modificare la transazione invalida la firma;
- anticipare la scadenza, perché i nodi la rifiutano;
- spendere i tuoi altri fondi, perché non ha le chiavi.

⚠️ **Però vede:**
- quali UTXO possiedi e quanto valgono;
- gli indirizzi degli eredi;
- la data in cui scatta l'eredità.

È un pezzo della tua mappa finanziaria in mano a terzi, un po' come condividere una [xpub](https://ortix.vercel.app/bitcoin/definizioni/blockchain/xpub/): i fondi non sono a rischio, la [privacy](https://ortix.vercel.app/bitcoin/filosofia/privacy/) sì. Un executor può anche sparire, chiudere, dimenticarsi o far trapelare i dati. Per questo conviene non affidarsi a uno solo.

## 🆚 Tre strade a confronto

| | Seed + lettera | Multisig | Transazioni a tempo (BAL/Àncòra) |
|---|---|---|---|
| Chi tiene le chiavi | Tu, finché la seed non viene trovata | Più persone o dispositivi | Solo tu |
| Rischio principale | Furto prima del tempo o seed mai trovata | Coordinamento, persone che spariscono | Rinnovo dimenticato, executor che vedono troppo |
| Cosa sanno i terzi | Tutto, se trovano la seed | Dipende dalla configurazione | UTXO, importi, eredi, scadenza |
| Manutenzione | Bassa | Media | Periodica: rinnovo obbligatorio |

Non c'è un vincitore. Sono strumenti che si possono **combinare**.

## ⚠️ Limiti e rischi

Nessuna di queste soluzioni è una garanzia assoluta. I punti deboli che vedo:

- **Il timer non distingue la morte dalla distrazione.** Se dimentichi di rinnovare, o sei vivo ma impossibilitato (un ricovero, un lungo viaggio senza accesso ai dispositivi), i fondi partono comunque.
- **Le fee si fissano oggi.** La commissione viene decisa al momento della firma. Se alla scadenza la [mempool](https://ortix.vercel.app/bitcoin/definizioni/blockchain/mempool/) è congestionata, la transazione può restare in attesa a lungo. Un erede esperto può accelerarla spendendo il proprio output con una fee più alta, ma deve saperlo fare.
- **I sats nuovi non sono coperti.** Gli UTXO ricevuti dopo la firma non fanno parte della transazione: va rifatta.
- **Il problema della custodia si sposta, non sparisce.** Gli eredi ricevono su wallet propri: devono saperli [creare](https://ortix.vercel.app/bitcoin/guide-e-consigli/come-creare-un-wallet-non-custodial/) e proteggerne la seed. La lettera di istruzioni serve ancora.
- **Fiducia nel software.** Un plugin tocca le tue transazioni. Don't trust, verify: controlla la provenienza, leggi la documentazione e prova prima con cifre piccole.
- **Privacy verso tutti i coinvolti.** Executor ed eredi sanno cosa riceveranno e quando.
- **La legge resta.** Una transazione a tempo non è un testamento e non sostituisce le norme sulla successione del paese in cui vivi.

## 🧪 Come la proverei, passo per passo

1. Un wallet di prova in Electrum con pochi sats, separato dal wallet principale.
2. Eredi di prova (anche un tuo secondo wallet) con indirizzi non custodial.
3. Una scadenza breve, per vedere il ciclo completo: firma, rinnovo, invalidazione della vecchia transazione.
4. Più executor indipendenti, per capire cosa ricevono e cosa vedono.
5. Solo dopo, valutare se e quanto affidare a questo sistema, e affiancarlo comunque a una lettera di istruzioni chiara.

## 🌳 Perché mi interessa

La sovranità non finisce con te. Un Bitcoin che nessuno sa recuperare è un patrimonio potato via per sempre. Le transazioni a tempo provano a tenere insieme due cose che sembravano in conflitto: **non consegnare le chiavi** e **non portarle nella tomba**. Hanno un costo in privacy e in disciplina, e va messo sul piatto con lucidità.

📎 Vedi anche: [Eredità in Bitcoin](https://ortix.vercel.app/bitcoin/eredita-in-bitcoin/), [⚡ Electrum](https://ortix.vercel.app/bitcoin/wallet/software-wallet/electrum/), [UTXO](https://ortix.vercel.app/bitcoin/definizioni/blockchain/utxo/), [🔐 Multisig](https://ortix.vercel.app/bitcoin/definizioni/blockchain/multisig/), [✍️ PSBT](https://ortix.vercel.app/bitcoin/definizioni/blockchain/psbt/), [🔐 Self-custody](https://ortix.vercel.app/bitcoin/definizioni/blockchain/self-custody/)
