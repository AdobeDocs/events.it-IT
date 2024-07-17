---
title: 'Ask the Expert - Follow-up to Workfront Proof Best Practices (Domande all’esperto: follow-up sulle best practice per)'
description: Scopri perché utilizzare i modelli di flusso di lavoro automatizzati, come crearli e come regolare le impostazioni della bozza per garantire la privacy. Questo webinar è stato registrato il 4 marzo 2020.
doc-type: feature video
team: Technical Marketing
kt: 9917
exl-id: 2b2f6522-2fd9-4d5e-9bc3-903c1d5e4e3b
duration: 4083
source-git-commit: 9a297cda953d4414131657f9ac84580aea0eabeb
workflow-type: tm+mt
source-wordcount: '1649'
ht-degree: 0%

---

# Ask the Expert - Follow-up to Workfront Proof Best Practices (Domande all’esperto: follow-up sulle best practice per)

Scopri perché utilizzare i modelli di flusso di lavoro automatizzati, come crearli e come regolare le impostazioni della bozza per garantire la privacy. Questo webinar è stato registrato il 4 marzo 2020.

>[!VIDEO](https://video.tv.adobe.com/v/341123/?quality=12)

## Domande e risposte

**Domanda**

Sembra che la nostra istanza generi automaticamente delle bozze durante il caricamento dei documenti. È possibile attivare/disattivare questa funzione?

**Risposta**

Sì, questa impostazione può essere disattivata all’interno del tuo profilo personale. Se fai clic su Impostazioni personali > Preferenze, è possibile selezionare o deselezionare la casella di controllo &quot;Genera automaticamente bozze durante il caricamento dei documenti&quot;.

**Domanda**

È possibile creare un flusso di lavoro con fasi vuote in modo da compilare singoli utenti dopo averlo associato per consentire a più team di utilizzare un flusso?

**Risposta**

Sì, i modelli di flusso di lavoro automatizzati possono avere fasi vuote in modo che, a seconda del team che lo utilizza, possano essere aggiunti utenti diversi.

**Domanda**

Nel nostro caso d’uso, l’autore carica il documento, ma l’account manager genera la bozza e imposta il flusso di approvazione. Quando è necessaria una nuova versione, la finestra di progettazione aggiunge la versione solo come documento e il processo riparte. Esiste un modo per far sì che l’account manager gestisca comunque il flusso delle bozze e che l’autore gestisca il controllo delle versioni senza dover generare il flusso ogni volta che si genera la nuova bozza?

**Risposta**

Se si imposta Designer con il livello di accesso Livello di lavoro o piano in Workfront, verrà concessa una licenza di verifica. Se la licenza di verifica è impostata su Supervisore o Amministratore, sarà possibile creare nuove versioni delle bozze senza dover eseguire la procedura manuale di conversione della nuova versione e applicazione di un flusso di lavoro. La nuova versione adotterà semplicemente il flusso di lavoro della versione precedente (e può anche essere modificata o modificata in questo momento).

**Domanda**

Cosa si consiglia per gli avvisi e-mail? decisioni o tutti gli avvisi?

**Risposta**

È consigliabile che il creatore/proprietario della bozza sia impostato su &quot;Decisioni&quot; per l’avviso e-mail. È consigliabile che tutti gli altri destinatari della bozza siano impostati su &quot;Disabilitato&quot; per l’avviso e-mail (anche se l’avviso e-mail è impostato su disabilitato, riceveranno comunque le notifiche New Proof, New Version, Late Proof e @Mention Email). Questa configurazione assicura che gli avvisi e-mail siano mirati e mantiene al minimo i messaggi e-mail.

**Domanda**

È possibile cambiare il proprietario della bozza che riceve una notifica quando vengono prese le decisioni? Si è tentato di utilizzare lo strumento di verifica, ma non è stato possibile cambiare il proprietario del documento da chi ha caricato il documento originale. Esempio: un marketing manager ha caricato il documento originale, ma è stato uno specialista di marketing a essere responsabile di prendere decisioni e apportare modifiche.

**Risposta**

Per cambiare il proprietario della bozza, segui il percorso: Documenti > Seleziona la bozza > Fai clic su &quot;Dettagli bozza&quot; > Nella finestra dei dettagli della bozza, individua il destinatario che desideri impostare come proprietario della bozza > Fai clic sul pulsante Idonei per quel destinatario e scegli &quot;Rendi proprietario&quot;.

**Domanda**

È stato rilevato il numero di turni di revisione?

**Risposta**

In genere, gli turni di revisioni corrispondono al numero di versioni della bozza.

**Domanda**

Una persona può trovarsi in più di una fase? In altre parole, se un manager in un ciclo di revisione iniziale ha la revisione finale in una fase successiva, come organizzeremmo questo?

**Risposta**

Anche se non è possibile aggiungere un destinatario della bozza a più di una fase di revisione di una bozza, una volta attivata la fase di revisione in cui si trova, il destinatario della bozza si troverà in tutte le fasi rimanenti per quella versione. Ciò consentirebbe loro di continuare a commentare e rispondere ai commenti anche se sono iniziate altre fasi. La chiave per assicurarsi che questo funzioni è assicurarsi che non si dispone di blocco stadi quando inizia la nuova fase.

**Domanda**

È possibile modificare i flussi di lavoro esistenti?

**Risposta**

Sì, puoi passare a Workfront Proof e selezionare Flussi di lavoro dal menu a sinistra. Qui è possibile modificare gli stadi, aggiungere utenti, rimuovere utenti, aggiungere stadi, ecc.

**Domanda**

È particolarmente utile disporre del flusso di lavoro di approvazione di un documento sulla bozza anziché sull’attività? È stata impostata per l&#39;attività di sviluppo di documenti e immagini, quindi se l&#39;immagine viene rifiutata in una qualsiasi fase del processo di approvazione, l&#39;attività torna in azione per consentire al progettista assegnato di modificarla. In questo modo, non dobbiamo lavorare in due luoghi. Ma forse mi manca qualcosa di importante su questa strada.

**Risposta**

Nel caso della verifica, si sta gestendo il processo di approvazione utilizzando il motore del flusso di lavoro della bozza. Questo consente di utilizzare lo strumento di revisione della bozza collaborativa per raccogliere feedback, commenti, markup, decisioni e fasi. È possibile utilizzare più attivatori del flusso di lavoro per instradare la bozza e impostazioni specifiche per le fasi della bozza, ad esempio Blocco, Fasi private e Responsabili delle decisioni primarie. Puoi anche assegnare ruoli di bozza univoci e notifiche e-mail di bozza univoche. Inoltre, puoi rivedere i contenuti in base alle diverse esigenze, ad esempio con bozze statiche, video e interattive (circa 150 tipi di file diversi).

**Domanda**

Chi può impostare il palcoscenico su un palcoscenico privato? Solo amministratori?

**Risposta**

La creazione del modello è responsabilità dell’amministratore, ma qualsiasi utente che può creare una bozza può renderla privata.

**Domanda**

La scadenza è inclusa nella notifica e-mail?

**Risposta**

Sì, se applichi una scadenza a una bozza, questa verrà visualizzata nella notifica e-mail.

**Domanda**

È possibile condividere un modello con un gruppo bozza?

**Risposta**

È possibile, tuttavia, tenere presente che verrà condiviso solo con i membri del gruppo che dispongono di licenze di verifica. Non potrai condividere modelli con utenti di Workfront o ospiti che non dispongono di licenze di verifica.

**Domanda**

In che modo una bozza viene reindirizzata al proprietario della bozza se viene rifiutata?

**Risposta**

Il proprietario della bozza rimane sulla bozza attraverso tutte le fasi di bozza. Se la bozza viene rifiutata, non è necessario inoltrarla nuovamente al proprietario. Al proprietario della bozza verrà invece inviata una notifica via e-mail della decisione presa, rivedi i commenti e inizia a utilizzare una nuova versione.

**Domanda**

Come disattivare/nascondere il documento &quot;Scarica&quot; in Proof?

**Risposta**

Quando aggiungi una nuova bozza, scorri verso il basso fino a quando non arrivi a Impostazioni bozza. Verrà visualizzata una casella di controllo per &quot;Scarica file originale&quot; che è possibile selezionare o deselezionare?

**Domanda**

In che modo questa impostazione di privacy in Impostazioni account influisce sugli utenti di verifica che utilizzano specificatamente il confronto automatico (affiancato a confronto automatico) — L&#39;impostazione predefinita DISabled impedisce al revisore di confrontare due versioni?

**Risposta**

Per l’impostazione di condivisione &quot;I destinatari possono visualizzare tutte le versioni&quot;: se è impostata su &quot;Disabilitata&quot;, se il destinatario non utilizzava la versione 1 ma la versione 2, non potrà confrontare le versioni 1 e 2. Si noti che gli utenti di Workfront con il livello di autorizzazione di bozza Supervisore o Amministratore saranno in grado di visualizzare tutte le versioni indipendentemente dall’impostazione.

**Domanda**

Possiamo avere diverse persone che caricano una nuova versione? ad esempio, un copywriter carica la versione 1 e poi abbiamo il correttore di bozza nella fase 1 . Vedono una modifica che deve essere fatta, può il caricamento versione 2?

**Risposta**

I destinatari della bozza possono creare nuove versioni di bozze se soddisfano i seguenti criteri: 1) sono i proprietari della bozza - o 2) dispongono del ruolo Autore o Moderatore della bozza - o 3) dispongono del livello di autorizzazione di bozza Supervisore o Amministratore.

**Domanda**

Come si gestiscono più bozze (ad es. A, B e C) con il flusso di lavoro automatizzato. Ricominciate?

**Risposta**

È possibile applicare un modello di flusso di lavoro automatico a più bozze al momento della creazione della versione iniziale. A questo scopo, segui il percorso: Documenti > Aggiungi nuovo > Bozza. Nella pagina Nuova bozza, seleziona più file da caricare, applica il modello di flusso di lavoro automatico e crea le bozze.

**Domanda**

È possibile esportare una bozza con commenti in un PDF?

**Risposta**

È possibile esportare un Riepilogo stampa su una bozza in un file PDF. Questo conterrà tutti i commenti, le annotazioni, le risposte e le decisioni.

**Domanda**

Dove posso visualizzare le impostazioni della bozza?

**Risposta**

Per visualizzare le impostazioni della bozza su una bozza esistente, segui il percorso: Scheda Documenti > Seleziona la bozza > Fai clic su &quot;Dettagli bozza&quot; > Dall’interno della finestra Dettagli bozza visualizzata, espandi l’area &quot;Impostazioni&quot;.

**Domanda**

Puoi assegnare un tag a qualcuno nella fase privata?

**Risposta**

Se sei un destinatario della bozza all’interno della fase privata, potrai assegnare tag a chiunque all’interno di tale fase privata. Se non sei nella fase privata, non potrai assegnare tag a qualcuno dall’interno della fase privata.

**Domanda**

Una volta attivata, è possibile disattivarla?

**Risposta**

Non sarà possibile disattivare una fase attiva, tuttavia, è possibile &quot;Bloccare&quot; la fase che impedirà alle persone all&#39;interno della fase di prendere commenti e decisioni.

**Domanda**

Cosa succede dietro le quinte quando uno o più revisori in un palco dicono che sono necessarie modifiche? Chi riceve una notifica per caricare una nuova versione?

**Risposta**

Questo dipenderà dall’impostazione &quot;Email Alert&quot; (Avviso e-mail) del creatore della bozza e/o dei destinatari della bozza sulla bozza. Consiglio ai Creatori/Proprietari della bozza di impostare l’avviso e-mail di &quot;Decisioni&quot; in modo che vengano notificate via e-mail in qualsiasi momento venga presa una decisione sulla bozza.
