WALLET 4.6 — GUIDA UTENTE
================================

Un'app per gestire le tue finanze personali direttamente dal browser.
Tutti i dati restano sul tuo dispositivo (nessun server, nessun cloud).


1. PRIMO AVVIO E SICUREZZA
----------------------------

All'apertura puoi scegliere se attivare la protezione con PIN a 4 cifre.

• PIN attivo → i dati vengono cifrati con AES-256-GCM e salvati in modo sicuro.
  ATTENZIONE: se dimentichi il PIN non c'è modo di recuperare i dati.
• PIN disattivato → i dati restano in chiaro sul dispositivo.

Blocco automatico: puoi impostare un timer (1 / 5 / 15 / 30 minuti) dopo il quale
l'app si blocca automaticamente se non la usi o se passi a un'altra scheda.

Dopo troppi tentativi errati il tastierino si blocca per 5 minuti.


2. LE 4 SCHERMATE PRINCIPALI
------------------------------

L'app si naviga scorrendo orizzontalmente o toccando le icone in basso:

A) 💸 CONTI (Liquidità)
   - Visualizza il saldo totale e l'elenco dei conti.
   - Registra entrate, uscite, spese fisse e programmate.
   - Cerca tra i movimenti recenti.

B) 🏦 PROGETTI (Risparmi)
   - Crea "salvadanai" per obiettivi (es. vacanze, emergenze).
   - Crea progetti con budget massimo per tracciare spese mirate.

C) 📈 INVESTIMENTI
   - Registra i tuoi investimenti (ETF, azioni, cripto...).
   - Tiene traccia del capitale investito.

D) 📊 STATISTICHE
   - Grafici interattivi: barre budget, % usata, entrate vs uscite, top 5 spese.
   - Genera e scarica report PDF.
   - Esporta / importa i dati, imposta i tetti di spesa.


3. COME REGISTRARE UN MOVIMENTO
---------------------------------

Dalla schermata "Conti":

• + ENTRATA → Aggiungi denaro a un conto (es. stipendio, rimborso).
• - SPESA   → Sottrai denaro da un conto. Scegli la categoria:
  - Essenziale (bollette, spesa, benzina...)
  - Passioni (hobby, sport, creatività...)
  - Svago / Extra (ristoranti, cinema, shopping...)

Puoi collegare ogni spesa a un Progetto per tracciarne l'andamento.


4. CONTI MULTIPLI
-------------------

Puoi creare più conti (es. Conto Corrente, Contanti, PayPal, Revolut...).
Ogni movimento è associato a un conto specifico.

Per creare un conto: tocca "+ CONTO" nella schermata Conti.
Per modificarlo o eliminarlo: usa i pulsanti ✎ e × accanto al nome.


5. SPESE FISSE E PROGRAMMATE
------------------------------

🔄 SPESE FISSE (Abbonamenti)
   - Registra pagamenti ricorrenti (Netflix, palestra, affitto...).
   - Se inserisci un "giorno di addebito" (1-31), l'app li registra
     automaticamente ogni mese nel conto scelto.
   - Senza giorno di addebito restano manuali: premi "Aggiungi" quando paghi.

📅 SPESE PROGRAMMATE
   - Inserisci spese future con data di scadenza (es. bollo auto, dentista).
   - L'app ti avvisa con un toast quando mancano 7 giorni o meno.
   - Quando paghi, premi il pulsante 💰 per confermare il pagamento e
     registrarlo come spesa effettiva.


6. RISPARMI E PROGETTI
------------------------

🏦 SALVADANAI
   - Crea obiettivi di risparmio con una cifra target.
   - Aggiungi denaro manualmente con il pulsante "AGGIUNGI".
   - Puoi scegliere se scalare l'importo da un conto (registrando
     automaticamente una spesa in categoria "Risparmio").

🎯 PROGETTI
   - Ideale per lavori, viaggi o acquisti mirati.
   - Assegna un budget massimo: la barra di avanzamento diventa rossa
     se superi il limite.
   - Le spese collegate al progetto vengono sommate automaticamente.


7. INVESTIMENTI
-----------------

Registra i tuoi asset finanziari per tenere traccia del capitale investito.
Questo valore è separato dalla liquidità e dai risparmi.


8. STATISTICHE E BUDGET
-------------------------

Nella schermata "Statistiche & Budget" puoi:

• Filtrare per periodo: Settimana / Mese / Anno / Sempre.
• Scegliere il tipo di grafico:
  - Barre Budget: confronta spese per categoria contro il tetto impostato.
  - Percentuale Usata: distribuzione a fette delle spese.
  - Entrate vs Uscite: bilancio del periodo.
  - Top 5 Spese: le uscite più pesanti.

⚙️ TETTI DI SPESA (Budget)
   - Imposta un limite per ogni categoria (Essenziale, Passioni, Svago).
   - Ogni categoria ha il proprio periodo: settimanale, mensile o annuale.
   - Quando raggiungi il 90% del budget ricevi un avviso toast.
   - Se superi il limite l'avviso diventa rosso.


9. REPORT PDF
---------------

Dalla schermata "Statistiche & Budget" tocca "📄 REPORT PDF" per generare
un report finanziario professionale da scaricare e condividere.

Periodi disponibili:
• Questa Settimana
• Questo Mese
• Ultimi 6 Mesi
• Quest'Anno

Il PDF include:
• Riepilogo: entrate totali, uscite totali e saldo netto.
• Ripartizione per Categoria: quanto hai speso in ogni categoria con percentuali.
• Andamento Mensile: entrate, uscite e netto mese per mese (se copre più di un mese).
• Saldi Conti Attuali: istantanea di tutti i tuoi conti al momento della generazione.

NOTA: il PDF viene generato interamente sul tuo dispositivo. La prima volta
serve una connessione internet per scaricare la libreria jsPDF dal CDN.
Dopo di che funziona anche offline.


10. IMPOSTAZIONI
------------------

Tocca l'ingranaggio ⚙️ in alto a destra.

• 💱 Valuta: cambia tra EUR, USD, GBP, CHF, JPY, CAD, AUD.
  Tutti gli importi vengono convertiti automaticamente con il tasso
  di cambio attuale (richiede connessione internet).

• 🌍 Lingua: Italiano / English.

• 🎨 Tema: Scuro, Chiaro, Oceano, Foresta.

• 👁️ Privacy: attiva la modalità "occhiolino" per nascondere
  tutte le cifre sensibili (mostra *** al posto degli importi).

• 🔒 Blocco automatico: scegli dopo quanto tempo di inattività
  l'app richiede nuovamente il PIN.

• 🔐 Protezione PIN: attiva, disattiva o cambia il PIN di sblocco.


11. BACKUP E RIPRISTINO
-------------------------

💾 ESPORTA
   - Scarica un file JSON con tutti i tuoi dati.
   - Se il PIN è attivo, il backup è anch'esso cifrato e protetto.

📁 IMPORTA
   - Carica un file JSON precedentemente esportato.
   - Se il backup è cifrato, ti verrà chiesto il PIN usato al momento
     dell'esportazione.
   - L'app avvisa se il backup che stai importando è più vecchio dei
     dati attuali sul dispositivo.

🗑️ SVUOTA CRONOLOGIA
   - Cancella tutti i movimenti (entrate, uscite, risparmi...).
   - I saldi dei conti restano invariati.
   - Utile per ripartire da zero senza ricreare i conti.


12. DOMANDE FREQUENTI
-----------------------

D: I miei dati sono al sicuro?
R: Sì, restano solo sul tuo dispositivo. Se attivi il PIN sono cifrati
   con AES-256-GCM. Nessuno (nemmeno lo sviluppatore) può accedervi.

D: Cosa succede se cancello i dati del browser?
R: Perdi tutto. Per questo è fondamentale fare regolarmente backup JSON.

D: Posso usarla offline?
R: Sì, tranne per il cambio valuta e la prima generazione di PDF che
   richiedono internet per recuperare risorse esterne.

D: Perché non vedo le notifiche del browser?
R: Devi autorizzare le notifiche quando il browser te lo chiede.
   Su iOS Safari le notifiche web push possono essere limitate.

D: Ho dimenticato il PIN. Cosa faccio?
R: Tocca "PIN dimenticato?" nella schermata di blocco.
   ATTENZIONE: questa azione cancella TUTTI i dati e reimposta l'app.
   Non c'è modo di recuperare i dati senza il PIN.

D: Posso modificare una transazione dopo averla inserita?
R: Sì, tocca il pulsante ✎ accanto al movimento nella lista.
   Puoi cambiare importo, descrizione, conto, categoria e progetto.


13. SUGGERIMENTI PRATICI
--------------------------

1. Crea subito i tuoi conti reali (Conto Corrente, Contanti...).
2. Imposta i budget mensili per avere il controllo delle uscite.
3. Usa i Progetti per spese importanti (viaggi, ristrutturazioni...).
4. Attiva le Spese Fisse con addebito automatico per non dimenticare
   mai un abbonamento.
5. Genera un report PDF prima di un incontro con la banca o il commercialista.
6. Esporta un backup JSON almeno una volta al mese.
7. Se usi il PIN, annotalo in un luogo sicuro (gestore password).


Buona gestione del budget! 💰
