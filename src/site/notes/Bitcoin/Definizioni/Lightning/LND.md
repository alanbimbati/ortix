---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/lightning/lnd/","title":"⚡ LND: Lightning Network Daemon","tags":["Bitcoin","Lightning","Definizione","Software","Node"],"dg-note-properties":{"title":"⚡ LND: Lightning Network Daemon","tags":["Bitcoin","Lightning","Definizione","Software","Node"],"aliases":["LND","Lightning Network Daemon"]}}
---


# ⚡ LND: Lightning Network Daemon

🧱 **LND** (Lightning Network Daemon) è una delle principali implementazioni del protocollo [[Bitcoin/Lightning Network/⚡ Lightning Network\|Lightning Network]], sviluppata da **Lightning Labs**. 

È il software (il "client") che gira su un computer o server domestico per gestire transazioni Lightning, aprire e chiudere [[Bitcoin/Definizioni/Lightning/Canale di Pagamento\|Canali di Pagamento]], calcolare percorsi di [[Bitcoin/Definizioni/Lightning/Routing\|Routing]] e salvaguardare lo [[Bitcoin/Definizioni/Lightning/Stato dei Canali\|Stato dei Canali]].

---

## 🎯 Il Framework di Responsabilità

1. **Chi decide?** LND è open-source. Gli sviluppatori propongono modifiche e aggiornamenti al codice, ma spetta all'operatore del nodo (tu) decidere quale versione far girare sul proprio server.
2. **Quali incentivi ha?** Ha l'incentivo a essere il software più stabile, sicuro e compatibile possibile. Supporta standard avanzati per consentire a wallet come [[Bitcoin/Lightning Network/Blixt\|Blixt]] e [[Bitcoin/Lightning Network/Zeus\|Zeus]] di interfacciarsi remotamente tramite credenziali sicure (Macaroon) e protocolli Tor/VPN.
3. **Chi è responsabile?** L'utente che fa girare LND è responsabile di aggiornare il client, monitorare lo stato del nodo fisso e assicurarsi che non si verifichino guasti al disco rigido che potrebbero corrompere il database di stato dei canali.
