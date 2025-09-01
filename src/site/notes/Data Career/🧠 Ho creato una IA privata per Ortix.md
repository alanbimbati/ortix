---
{"dg-publish":true,"permalink":"/data-career/ho-creato-una-ia-privata-per-ortix/","title":"🤖 Progetto AI Vault Ortix - Resoconto","tags":["AI","LLM","Obsidian","llama_index","localAI","embedding","ETL","Sovranità Digitale"]}
---

# 🧠 Ho creato una IA privata per Ortix

![Pasted image 20250801183101.png](/img/user/Immagini/Pasted%20image%2020250801183101.png)

🌱 **Ortix** è il mio giardino digitale, uno spazio dove conservo tutta la mia conoscenza, idee e riflessioni.  
Da tempo sognavo di poterci *parlare* direttamente, come se fosse una mente secondaria sempre disponibile, **senza passare da ChatGPT, Gemini o altri servizi esterni**.  
In una parola: **una IA tutta mia**, in locale, senza internet, nel pieno rispetto della mia **[[Ortix/Filosofia/🛡️ Sovranità digitale\|🛡️ Sovranità digitale]]**.

---

## ⚙️ Cosa ho fatto

💾 Ho usato **#Python** per scrivere un piccolo programma che:
- Legge tutti i miei file Markdown di Ortix
- Li trasforma in un formato comprensibile per una IA (embedding)
- Li collega a un **modello LLM locale**, che può rispondere in linguaggio naturale

🧠 All’inizio ho scaricato due modelli:  
- uno per *capire* il contenuto (`all-MiniLM`, molto leggero, ottimo per trasformare i testi in vettori),  
- uno per *rispondere* alle domande (`llama-3-8b-instruct`, un grande modello linguistico locale, da usare al posto di ChatGPT).

![Pasted image 20250801182941.png](/img/user/Immagini/Pasted%20image%2020250801182941.png)

👎🏻 Al primo tentativo, **ha funzionato**... ma:
- ci ha messo **6 minuti per rispondere**,
- **solo in inglese**!

---

## 🛠 Come l’ho migliorata

🔧 Ho allora:
- Scaricato un **modello più leggero**, adatto al mio PC di 5 anni fa
- Aggiunto un **system prompt** per dirgli di rispondere sempre in italiano e in modo chiaro

![Pasted image 20250801182954.png](/img/user/Immagini/Pasted%20image%2020250801182954.png)

✅ Così facendo, ho ottenuto un assistente in grado di leggere Ortix e rispondere alle mie domande.  
Certo, una risposta può richiedere anche **3 minuti**, ma funziona! E **tutto in locale**.

---

## 🧪 Quale modello scegliere?

📊 Ecco una tabella con le principali opzioni che ho testato, con RAM minima, velocità e qualità:

| Modello GGUF          | RAM Minima  | Velocità CPU | Qualità       |
|------------------------|-------------|--------------|----------------|
| `llama-3-8b Q4_K_M`    | 20+ GB      | 🐢 Lento     | 🔥 Alta        |
| `mistral-7b Q4_K_M`    | 12 GB       | 🐌 Media     | 🔥 Alta        |
| `phi-2 Q4_K_M`         | 6–8 GB      | ⚡️ Veloce    | 👍 Buona       |
| `llama-3-8b Q2_K`      | 10–12 GB    | ⚠️ Più veloce | 😐 Qualità bassa |

💡 La scelta dipende dal tuo hardware e dai tuoi obiettivi: qualità, velocità o leggerezza.

---

## 🎓 Cosa ho imparato

- Non serve un super computer per costruire una IA personale
- Esistono modelli gratuiti e [[Bitcoin/🧬 Open Source\|🧬 Open Source]] che puoi usare liberamente
- È **possibile creare un assistente privato** partendo solo da qualche nozione di Python
- Una volta impostato il sistema, posso **cambiare modelli, migliorare le risposte**, oppure usare plugin Obsidian per automatizzare tutto

---

📍 È stato un esperimento istruttivo e stimolante.  
Ora posso chiedere a Ortix *“Cos'è un Full Node?”* e lui mi risponde…  
con calma 😅, ma **senza spiare nulla a nessuno**.

---

[[Data Career/🧠 Da Data Manager a giardiniere digitale\|🧠 Da Data Manager a giardiniere digitale]]

#Ortix #AI #LLM #LocalAI #Obsidian #Python #SovranitàDigitale
