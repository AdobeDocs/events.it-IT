---
title: 'Chiedi all’esperto: best practice per massimizzare la bozza di Workfront'
description: Scopri come configurare le impostazioni, abilitare funzioni di reporting avanzate ed evitare problemi comuni in Proof. Questo webinar è stato registrato il 26 febbraio 2020.
doc-type: feature video
team: Technical Marketing
kt: 9916
exl-id: 7d3e437d-4a6e-44b8-9eff-eabb8284c391
duration: 5182
source-git-commit: 9a297cda953d4414131657f9ac84580aea0eabeb
workflow-type: tm+mt
source-wordcount: '5572'
ht-degree: 2%

---

# Chiedi all’esperto: best practice per massimizzare la bozza di Workfront

Scopri come configurare le impostazioni per il successo, accedere alle visualizzazioni (e altri trucchi) per abilitare funzioni di reporting avanzate e come evitare le insidie più comuni in Proof. Questo webinar è stato registrato il 26 febbraio 2020.

>[!VIDEO](https://video.tv.adobe.com/v/341122/?quality=12)

## Domande e risposte

**domande**

Attualmente, per consentire a un destinatario di condividere una bozza condivisa con lui, è necessario selezionare manualmente la casella &quot;subscription&quot; in proof settings. Per impostazione predefinita, è prevista l&#39;esecuzione automatica di questa casella?

**Risposta**

Per abilitare/disabilitare questo valore come impostazione predefinita per i singoli utenti, un amministratore può seguire questo percorso: Accesso PHQ > Impostazioni account > Utenti > Fai clic sul nome dell’utente > Impostazioni bozza predefinite.

**domande**

Se non selezioni &quot;Nuova bozza&quot; e carichi un documento e l’utente è impostato su &quot;genera automaticamente la bozza&quot;. È possibile modificare tali impostazioni dopo che i file sono già stati caricati?

**Risposta**

Sì.  Per regolare tutte le impostazioni della bozza, seleziona la bozza nella scheda Documenti e fai clic su Dettagli bozza.

**domande**

Questa presentazione è applicabile allo strumento autonomo?

**Risposta**

Le impostazioni di Recommendations on Proof Roles (Ruoli bozza), Email Alerts (Avvisi e-mail), Decision Options (Opzioni di decisione), Forwarding Emails (Inoltro e-mail) e Workflow Template Grouping (Raggruppamento/Condivisione/Condivisione di modelli di flusso di lavoro) sono tutte rilevanti per Proof standalone.

**domande**

Per cosa si utilizza un modello di bozza?

**Risposta**

Se il processo di revisione del contenuto dell’organizzazione viene spesso ripetuto o il contenuto viene spesso rivisto dalle stesse persone, è possibile creare modelli di flusso di lavoro che contengano tali revisori con i ruoli delle bozze e le impostazioni di notifica specificati.

**domande**

Cos’è un modello di flusso di lavoro di una bozza?

**Risposta**

Un modello di flusso di lavoro di una bozza è un modello con un flusso di lavoro di instradamento della bozza predeterminato che può essere applicato alle bozze. Consentono di standardizzare e automatizzare i processi di approvazione delle bozze.

**domande**

Come si crea un modello di bozza?

**Risposta**

In qualità di amministratore, dovrai seguire questo percorso: Accesso PHQ > Flussi di lavoro > Nuovo > Nuovo modello.

**domande**

Questa funzionalità di condivisione dei modelli consente la condivisione con gruppi e team o solo con singoli utenti?

**Risposta**

Al momento non è possibile condividere i modelli di flusso di lavoro con Workfront Groups, Teams, Job Roles o Companies. Tuttavia, puoi condividerli con singoli utenti e con Gruppi di bozze. Per creare un gruppo bozza, segui questo percorso: Accesso PHQ > Gruppi > Nuovo gruppo.

**domande**

Quando si invia una bozza, in Organizzazione, è possibile pulire le cartelle visualizzate da ogni utente in modo che visualizzino solo le cartelle applicabili? Invece di tutte le cartelle che sono state create all&#39;interno dell&#39;account aziendale?

**Risposta**

Questa domanda è relativa alla versione standalone di Workfront Proof. All’interno di Workfront Proof standalone puoi utilizzare le Cartelle private per nascondere le cartelle a utenti specifici. In questo modo sarà possibile scegliere un elenco più semplice di cartelle. Puoi anche utilizzare la logica di completamento automatico per individuare la cartella a cui desideri aggiungere una bozza.

**domande**

I revisori e gli approvatori hanno la possibilità di modificare queste impostazioni di notifica?

**Risposta**

Gli amministratori di Workfront possono modificare le impostazioni predefinite degli avvisi e-mail per utenti e contatti. I creatori di bozze possono quindi modificare l’impostazione di notifica durante la creazione di una bozza e sulle bozze esistenti.

I destinatari delle bozze possono sempre modificare il proprio avviso e-mail per specifiche bozze a livello di bozza all’interno dello strumento Proof Viewer (Visualizzatore di bozze) selezionando l’icona Impostazioni nel menu a sinistra.

**domande**

Gli avvisi e-mail sostituiscono le notifiche globali?

**Risposta**

Gli avvisi e-mail relativi alle bozze sono completamente indipendenti dalle impostazioni globali di notifica.

**domande**

Se i revisori sono impostati su &quot;disabilitato&quot;, come sapranno se c&#39;è una nuova bozza da rivedere se hanno rifiutato una precedente?

**Risposta**

Gli avvisi e-mail sono indipendenti da E-mail New Proof (Nuova bozza), E-mail New Version (Nuova versione), E-mail At Risk (A rischio), E-mail Late (In ritardo) e E-@Mentions. Se scegli &quot;Disabilitato&quot; come avviso e-mail, disabiliterai solo le notifiche di attività come commenti, risposte e decisioni sulla bozza (ad eccezione delle e-mail @Mention dai commenti).

**domande**

L’impostazione Disattiva e-mail si applica a tutto il sistema Enterprise? o è per Portfolio?

**Risposta**

L’impostazione che si trova in Configurazione > E-mail > Revisione e approvazione e che abilita/disabilita l’invio delle e-mail quando i destinatari della bozza presentano commenti è Enterprise Wide (si tratta di un’impostazione globale).

**domande**

Un utente &quot;Guest&quot; aggiunto alla bozza non può esaminarla. L’utente non dispone dell’accesso in Workfront.

**Risposta**

Se il Guest può accedere alla bozza ma non prendere commenti/decisioni, assicurati di controllare il suo Ruolo bozza nella bozza. In questo caso, è possibile che siano state aggiunte alla bozza con il ruolo &quot;Sola lettura&quot;. Se sulla bozza sono impostati come revisore o revisore e approvatore e non possono ancora fare commenti/markup/decisioni, invia un ticket di supporto.

**domande**

Gli utenti guest richiedono una licenza?

**Risposta**

Gli utenti guest non richiedono una licenza.

**domande**

Non vedo la casella di decisione della bozza?

**Risposta**

Se la casella di decisione bozza non viene visualizzata su una bozza, è possibile che sulla bozza sia impostato il ruolo di bozza Sola lettura o Revisore oppure che la fase in cui ci si trova non sia ancora iniziata.

**domande**

È possibile chiarire l’impostazione in WF>Configurazione - se si dispone dell’opzione su per inviare e-mail per ogni commento - questi vengono inviati anche se l’e-mail in PHQ è disabilitata? e chi riceve le e-mail??

**Risposta**

L’opzione Workfront Setup > E-mail > Revisione e approvazione notifica è indipendente dalle opzioni di Avviso e-mail a livello di bozza. Se questa opzione è abilitata, a tutti gli utenti di ogni bozza verrà inviata un’e-mail ogni volta che qualcuno tra le bozze in cui si trovano aggiunge un commento.

**domande**

In precedenza avevi consigliato di disattivare per gli avvisi e-mail al di fuori del proprietario della bozza. I destinatari riceveranno ancora una notifica e-mail che indica che in tal caso è stata loro assegnata una bozza?

**Risposta**

Sì.  Gli avvisi e-mail (che possono essere impostati su Tutte le attività, Disattivato, Decisioni ecc.) sono indipendenti dalle e-mail di notifica della bozza (Nuova bozza, Nuova versione, A rischio, Bozza in ritardo, @Mentions).

**domande**

Cosa succede se hai un&#39;istanza in cui qualcuno viene aggiunto a una bozza e si sente come se non dovesse essere lì? La rimozione di &quot;Non pertinente&quot; non consentirebbe di scegliere un&#39;opzione?

**Risposta**

Questo è un buon utilizzo per l’opzione di decisione non rilevante. Tuttavia, se qualcuno non dovesse comparire sulla bozza, ti consiglierei di @Mention il proprietario della bozza in un commento e di chiederne la rimozione. Se qualcuno che deve prendere una decisione sulla bozza prende una decisione di &quot;Non rilevante&quot; quando deve prendere una decisione di Approvato o Modifiche richieste, ciò potrebbe alterare il funzionamento del flusso di lavoro applicato a quella bozza.

**domande**

Dove si trova la casella di controllo &quot;Richiedi accesso&quot; per gli utenti guest?

**Risposta**

Questo si trova in Impostazioni bozza nella pagina Creazione bozza al momento della creazione di una bozza. Se la bozza è già stata creata, puoi accedere a questa impostazione selezionando la bozza nella scheda Documenti e facendo clic su Dettagli bozza > Impostazioni. Puoi condividere le bozze Login Required solo con persone che dispongono di una licenza Proofing.

**domande**

Qualcuno può rimuovere se stesso da una bozza se è stato aggiunto da qualcun altro?

**Risposta**

Se la persona dispone dei diritti di modifica per la prova a cui è stata aggiunta può rimuoversi. Le persone con diritti di modifica saranno Utenti Workfront con una licenza di verifica di livello Amministratore o Supervisore, nonché persone aggiunte alla bozza con i ruoli di bozza Autore o Moderatore. Chiunque altro dovrà essere rimosso da un utente con diritti di modifica.

**domande**

Perché dovrei usare l&#39;approvazione documento e l&#39;approvazione bozza o viceversa?

**Risposta**

Approvazione documento può essere utilizzato per un documento che non richiede commenti e markup in linea con il documento da approvare. Ad esempio, ho solo bisogno che guardi questo documento e che lo approvi o lo rifiuti. La bozza consentirà l’inserimento di commenti e markup all’interno del documento nello strumento Proof Viewer (Visualizzatore di bozze). Ad esempio, ho bisogno che tu guardi questa bozza, aggiunga commenti, aggiunga markup e prenda una decisione. In futuro, il piano è quello di unificare le due funzionalità in quanto sono molto simili.

**domande**

Siamo un reparto Marketing e approviamo una bozza interna, quindi dobbiamo inviarla esternamente al richiedente. Non diamo accesso ai richiedenti ai nostri progetti. Inoltre, non vogliamo che vedano tutti i nostri commenti nella bozza interna. Ora stiamo creando una nuova bozza pulita, la stiamo scaricando e inviando loro via e-mail. Vogliamo che utilizzino Proof HQ, ma non siamo sicuri di come farlo senza che questo dia loro anche l’accesso al nostro progetto. Hai qualche suggerimento?

**Risposta**

È consigliabile utilizzare i modelli di flussi di lavoro automatizzati, che consentono di utilizzare &quot;Fasi private&quot;. Le fasi private consentono di nascondere i commenti, le annotazioni e le decisioni dei revisori ospiti in altre fasi. In questo modo, la revisione della bozza interna potrebbe essere completamente nascosta al richiedente esterno.

**domande**

Una volta creata una bozza da un altro utente, qual è il modo migliore per aggiungerti in qualità di revisore e approvatore?

**Risposta**

Se sei un utente di Workfront con l’autorizzazione Verifica dell’amministratore o del supervisore, puoi aggiungere te stesso o te stessa come revisore e approvatore a qualsiasi bozza a cui hai accesso. In caso contrario, sarà necessario chiedere l’aggiunta del proprietario della bozza (o di un altro utente con diritti di modifica sulla bozza).

**domande**

Abbiamo tentato di assegnare tag agli utenti in una bozza, ma non ricevono una notifica e-mail. Nelle impostazioni dell’account è presente un elemento per assicurarsi che venga inviato un messaggio e-mail?

**Risposta**

Ti consigliamo di controllare Filtri e-mail/Cartella spam per verificare se le notifiche sono andate lì e quindi apportare le modifiche necessarie all’interno dell’applicazione e-mail per inserire in una whitelist tali e-mail. Puoi anche contattare il nostro team di supporto con assistenza al riguardo.

**domande**

È possibile @ qualcuno solo se hanno una licenza Verifica, corretto? Come in, questa persona non è mai stata inclusa nella bozza e desideri assegnarle un tag (@).

**Risposta**

Se sei un ospite o un utente di Workfront con una licenza di verifica di Manager puoi @Mention chiunque si trovi sulla bozza (indipendentemente dal fatto che la persona disponga o meno di una licenza). Se sei un utente di Workfront con una licenza di verifica del supervisore o dell’amministratore oppure sei il proprietario della bozza, puoi @Mention chiunque si trovi all’interno dell’elenco contatti nella piattaforma di verifica.

**domande**

Problema principale: indirizzo e-mail %2B (indirizzi e-mail duplicati). Perché e come si verifica e come si può porvi rimedio?

**Risposta**

Questo può accadere se qualcuno aggiunge manualmente qualcuno a una bozza utilizzando l’indirizzo e-mail errato. In questo caso, un amministratore può rimuovere l’indirizzo e-mail errato dall’account Proof seguendo questo percorso: Accesso PHQ > Contatti > Seleziona l’istanza e-mail/ospite errata > Elimina. In caso di problemi con gli utenti che vengono aggiunti con indirizzi e-mail duplicati, contatta il nostro team di supporto per assistenza.

**domande**

Una volta presa la decisione, devi cambiare la bozza in produzione. Che tipo di accesso devi fornire al team di produzione in modo che possa utilizzare l’azione del commento se la bozza è bloccata?

**Risposta**

Se una bozza è bloccata, sarà necessario sbloccarla per consentire agli utenti di inviare commenti sulle azioni o rispondere ai commenti. Le persone con le seguenti autorizzazioni possono sbloccare la bozza: Proprietario bozza, Utenti Workfront con un Livello di licenza bozza di Amministratore o Supervisore.

**domande**

Qual è la soluzione migliore per i team per conoscere le bozze già in coda?

**Risposta**

Puoi creare un rapporto Proof Approvals (Approvazioni bozza) all’interno di Workfront. Puoi quindi applicare filtri che visualizzino solo le bozze per utenti specifici che richiedono ancora di essere decisi.

**domande**

Esiste un modo per scaricare le bozze con le relative approvazioni associate in una cartella?

**Risposta**

È possibile accedere e scaricare un rapporto Stampa riepilogo per le bozze che includerà tutti i commenti, le risposte, i markup, le azioni e le decisioni in tutte le versioni.

**domande**

Quando si richiede agli utenti di accedere alla segnalazione di ProofHQ, questo concederà loro anche l’accesso alla sezione a sinistra (ad es. flussi di lavoro, contatti, impostazioni account, ecc.)?

**Risposta**

Questo dipenderà dal loro livello di licenza di bozza. Se sono configurate con la licenza Manager o Supervisore, potranno accedere ai Contatti ma non alle Impostazioni account e ai Flussi di lavoro. Se sono configurati con la licenza di amministratore, avranno accesso alle Impostazioni account e ai Flussi di lavoro.

**domande**

Nella mia organizzazione, il Project Manager invia la richiesta di approvazione alle parti interessate per la revisione o i commenti. Hai menzionato che non dovremmo aggiungere nomi ai campi di approvazione, come puoi tu, in quanto Primo Ministro, condividere la bozza creativa con le parti interessate?

**Risposta**

Il campo Approvazione è per Approvazioni documenti, che è adatto da utilizzare se si richiede solo una semplice approvazione del documento. Se desideri un’approvazione della bozza (con commenti, markup e una decisione di bozza), aggiungi le parti interessate alla bozza con il ruolo di bozza Revisore e Approvatore.

**domande**

Come si aggiungono persone come nuovi ruoli a una bozza già creata?

**Risposta**

Per aggiungere destinatari della bozza e selezionare il loro ruolo di bozza su una bozza esistente, segui questo percorso: seleziona la bozza nella scheda documenti > quindi fai clic su in Dettagli bozza. Quando viene visualizzata la finestra dei dettagli della bozza, fai clic sul pulsante Idonei in alto a destra nell’area di visualizzazione e seleziona &quot;Condividi&quot;. Potrai quindi aggiungere i destinatari e selezionare il loro ruolo di bozza e l’avviso e-mail.

**domande**

Se concediamo l’accesso a Proof HQ a responsabili/creatori di bozze, possiamo bloccare le aree di amministrazione come flussi di lavoro, gruppi, ecc.?

**Risposta**

Sì, è determinato dall&#39;autorizzazione di bozza utenti. Gli utenti con l’autorizzazione Verifica del Manager o del Supervisore non avranno accesso alle impostazioni account e ai modelli di flusso di lavoro. Gli utenti con l’autorizzazione Verifica dell’amministratore avranno accesso alle Impostazioni account e ai Modelli di flusso di lavoro. Tutti gli utenti con accesso potranno accedere all’area Gruppi.

**domande**

In che modo gli utenti possono visualizzare tutte le bozze a cui sono assegnati senza essere un proof manager?

**Risposta**

Se un utente desidera visualizzare tutte le prove su cui deve ancora prendere una decisione, può utilizzare l’area Home o My Updates (I miei aggiornamenti) in Workfront (a seconda del suo livello di accesso). Puoi anche creare un rapporto Proof Approval (Approvazione della bozza) e applicare filtri per mostrare solo le bozze di come l’utente connesso è un revisore e un approvatore.

**domande**

Ciao, puoi passare in rassegna i flussi di lavoro di verifica automatizzata, per le situazioni in cui sono presenti 3 cicli di progettazione e feedback, e come adattarli per i casi in cui il feedback viene fornito in ritardo, e come è possibile legarlo al meglio alle attività in WF per ogni ciclo (feedback di progettazione e project manager)?

**Risposta**

È possibile utilizzare diversi approcci per l&#39;utilizzo delle attività, oltre a quelli di revisione e approvazione. Un approccio che mi piace adottare è quello di avere un’attività per &quot;Instradamento bozza&quot; e utilizzo il flusso di lavoro bozza per gestire le notifiche ai destinatari (invece di assegnare loro un’attività). È quindi possibile creare un task per &quot;Ciclo di instradamento bozza 2&quot; e &quot;Ciclo di instradamento bozza 3&quot; che consente di tenere traccia del numero di arrotondamenti eseguiti. Potrai anche tenere traccia dell’avanzamento delle bozze utilizzando la dashboard bozze (accesso PHQ > dashboard > bozze da gestire). Questa visualizzazione indica il numero di bozze in ritardo (nonché di bozze a rischio) che si stanno gestendo.

**domande**

Quando viene eliminata una bozza, una copia della bozza è ancora presente sui server?

**Risposta**

Sì.  Se elimini una bozza, questa si trova nell’area Cestino dell’account di bozza associato. Se necessario, può essere ripristinata da lì e rimarrà lì fino a quando e a meno che il cestino non venga svuotato.

**domande**

Esiste un modo per attivare la nuova decisione se un altro utente rifiuta o approva con modifiche. Sì. Il team addetto alle bozze vede qualcosa, quindi il project manager dovrà prendere una nuova decisione, anche se l&#39;ha già esaminata e approvata. (cercando di non rendere il responsabile di progetto non deve aspettare il reparto bozze per fare la loro revisione)?

**Risposta**

Anche se questo non può essere automatizzato, puoi impostare Project Manager con l’avviso e-mail delle decisioni. In questo modo, quando il reparto di correzione prende la sua decisione, il Project Manager viene informato della decisione presa e può quindi tornare alla bozza, rivedere i commenti fatti dal reparto di correzione e quindi modificare la decisione, se necessario.

**domande**

Perché quando controllo &quot;Richiedi approvazione&quot; quando invio un aggiornamento nella sezione Dettagli bozza, visualizzo solo lo stato SOC e non SOCD. È consigliabile evitare di utilizzare questa casella di controllo? Qual è la best practice per inviare un aggiornamento su una bozza.

**Risposta**

Quando si utilizza la funzione &quot;Richiedi approvazione&quot;, si utilizza la funzionalità Approvazione documento che sarà indipendente da Strumenti di correzione e dalla barra di avanzamento SOCD. Se devi aggiornare il ruolo di bozza di un destinatario della bozza, segui questo percorso: dalla scheda Documenti, seleziona la bozza > quindi fai clic su Dettagli bozza. Quando viene visualizzata la finestra dei dettagli della bozza, viene visualizzato l’elenco dei destinatari e l’opzione relativa al ruolo della bozza (oltre all’avviso e-mail) può essere regolata in linea. Questo ti consente di (ad esempio) modificare il ruolo della bozza da Revisore a Revisore e Approvatore.

**domande**

È possibile garantire che gli approvatori finali non abbiano accesso alle versioni precedenti (e ai commenti) se sono presenti nello stesso documento di prova? È necessario creare un nuovo documento di bozza o esiste un modo per mantenere tutte le versioni e i commenti in un&#39;unica versione e designare l&#39;accesso alle versioni?

**Risposta**

Nelle Impostazioni account all’interno di proof (Bozza) puoi controllare la condivisione e la visibilità dell’accesso alle bozze. Per aggiornare questa impostazione in modo che i destinatari della bozza vedano solo le versioni delle bozze designate (invece di visualizzare tutte le versioni della bozza), dovrai seguire questo percorso: Accesso PHQ > Impostazioni account > Impostazioni > Condivisione > I destinatari possono visualizzare tutte le versioni = Disabilitato.

**domande**

È possibile aggiungere la schermata del dashboard bozze come pagina esterna a un dashboard WF? Gli utenti che non sono amministratori visualizzeranno la dashboard?

**Risposta**

Puoi aggiungere il dashboard di bozze come pagina esterna all’interno di un dashboard. Tieni presente che questo sarebbe visibile solo dagli utenti con una licenza di verifica.

**domande**

Le funzioni Dashboard e Reporting in ProofHQ sono disponibili solo per gli amministratori che hanno accesso a Proof, giusto? Non sono i responsabili della pianificazione generali che non hanno accesso come amministratori?

**Risposta**

Questo è corretto. È tuttavia possibile inviare un caso di supporto con Workfront per richiedere che tutti gli utenti con licenza di verifica abbiano accesso al sistema di verifica.

**domande**

Ciao, una domanda sulla flessibilità della proprietà della bozza: se è necessario caricare una nuova versione di bozza in assenza del proprietario originale, è la best practice per loro di aggiungere un collega al flusso di lavoro come autore e decideranno &quot;Non rilevante&quot;? La delega della proprietà sembra funzionare solo per una singola versione.

**Risposta**

Questo caso d’uso e questo flusso di lavoro funzionerebbero perfettamente. Un’altra cosa che potresti considerare, tuttavia, è richiedere agli utenti che potrebbero aver bisogno di caricare nuove versioni nelle bozze che non sono i proprietari di essere impostati con il Livello di autorizzazione di bozza di Supervisore o Amministratore. Questo livello di autorizzazione consente loro di caricare nuove versioni nelle bozze di di cui non sono proprietari senza doverle aggiungere alla bozza come Autore o Moderatore (il che richiederebbe una decisione per entrambi).

**domande**

Per come la vedo io, non puoi aggiungere lo stesso utente nelle fasi successive di un flusso di lavoro automatizzato, e questo per noi è problematico. È qualcosa che puoi modificare per consentire allo stesso utente di essere in più fasi?

**Risposta**

Anche se non è possibile aggiungere un destinatario della bozza a più di una fase di revisione di una bozza, una volta attivata la fase di revisione in cui si trova, il destinatario della bozza si troverà in tutte le fasi rimanenti per quella versione. Ciò consentirebbe loro di continuare a commentare e rispondere ai commenti anche se sono iniziate altre fasi. La chiave per assicurarsi che questo funzioni è assicurarsi di non avere blocchi di stadi quando iniziano nuovi stadi.

**domande**

È possibile spiegare l’instradamento delle bozze tra le fasi? Come è possibile chiuderne uno e passare alla fase successiva?

**Risposta**

Sono disponibili alcune opzioni nei modelli di flusso di lavoro automatizzati che consentiranno al di passare da una fase all’altra. Le opzioni che è possibile utilizzare includono &quot;Creazione in bozza&quot;, &quot;Quando tutte le decisioni sono approvate in una fase padre&quot; &quot;Quando tutte le decisioni sono approvate o approvate con modifiche in una fase padre&quot;, &quot;Quando tutte le decisioni sono prese in una fase padre&quot; e alcune altre opzioni.

**domande**

È possibile rimuovere una bozza da un documento generato automaticamente, ma non si desidera che sia una bozza?

**Risposta**

Se è attivata l’impostazione &quot;Genera automaticamente bozze durante il caricamento dei documenti&quot;, non sarà possibile rimuovere una bozza da un documento. Sarà invece necessario ricaricarlo tramite il pulsante Aggiungi nuovo > Documenti.

**domande**

Un utente può dire nella fase 3 del flusso della bozza di aggiungere un’altra persona come Revisione e Approvatore?

**Risposta**

Se tale utente dispone dei diritti di modifica sulla bozza, può farlo. Le persone con diritti di modifica saranno: Proprietario bozza, Destinatari bozza aggiunti alla bozza con il Ruolo bozza Autore o Moderatore, Utenti con licenza bozza con il Livello di autorizzazione bozza Supervisore o Amministratore.

**domande**

Se un utente viene designato come autore, può caricare una nuova versione della bozza? Non si tratta del creatore della bozza.

**Risposta**

I destinatari della bozza con il ruolo di bozza Autore e Moderatore possono aggiungere nuove versioni alle bozze a cui appartengono con tale ruolo.

**domande**

Gli utenti esterni ricevono un’e-mail per bozza da rivedere. Questo può essere difficile per loro di tenere traccia dello stato di tutte le prove che hanno in gioco. Esistono dashboard o opzioni di elenchi di stati e-mail o prossime funzionalità per gli utenti esterni per monitorare il proprio stato su più bozze?

**Risposta**

È consigliabile aggiungere questi utenti esterni a Workfront con una licenza Revisore gratuita. Questo consentirà loro di accedere a una pagina I miei aggiornamenti che includerà un elenco di tutte le prove in sospeso necessarie per prendere una decisione su.

**domande**

Puoi spiegare di più sulle notifiche delle decisioni? Riceverò notifiche solo con i commenti della bozza da Revisori e Approvazioni o riceverò anche i commenti dai Revisori e quando li riceverò?

**Risposta**

Le notifiche degli avvisi e-mail sulle decisioni vengono inviate solo quando vengono prese decisioni sulla bozza. Non saranno inviate al momento in cui vengono formulate le osservazioni. Tuttavia, se ricevi un avviso e-mail di decisione che indica che un destinatario sulla bozza ha preso una decisione di Modifiche richieste, saprai che è il momento giusto per rivedere i commenti aggiunti (che si troveranno nella bozza).

**domande**

Per quanto riguarda il problema dell’inoltro delle e-mail, stai effettuando l’accesso come proprietario dell’e-mail? E questo accadrebbe in ambienti chiusi a chiave? Si verificherebbe con un ambiente SSO?

**Risposta**

In questo modo, accedi alla bozza come persona che ti ha inoltrato l’e-mail. L’utilizzo di Accesso richiesto per le bozze e di SSO impedisce l’accesso alla bozza in qualità di persona che ti ha inoltrato l’e-mail.

**domande**

Dove posso accedere alla dashboard e ai report nella verifica?

**Risposta**

Se disponi di un’icona a forma di casella di controllo a destra della barra di ricerca in Workfront, significa che disponi di un account Workfront e Proof integrato. Selezionando la casella di controllo, si aprirà Workfront Proof e la dashboard verrà visualizzata nella schermata iniziale. I rapporti possono essere creati utilizzando l’opzione Viste nel pannello a sinistra.

**domande**

Nella sezione &quot;Ruolo&quot;, ci sono 2 segni di spunta in basso che indicano che stai per aggiungere qualcuno utilizzando un @mention, ecc. Nelle impostazioni della bozza puoi impostare ruoli predefiniti per ogni persona, ma non è possibile far controllare automaticamente tali segni di spunta, pertanto è necessario farlo ogni volta che crei una bozza. Come puoi impostare questa impostazione come predefinita per un utente?

**Risposta**

Attualmente non esiste un modo per impostare questa come impostazione predefinita per i destinatari della bozza. Tuttavia, è possibile salvarli come impostazioni predefinite per i destinatari all’interno di Modelli di flusso di lavoro automatizzati.

**domande**

Come si cambia il proprietario di una bozza?

**Risposta**

Per cambiare il proprietario di una bozza, segui il percorso indicato di seguito: Nella scheda Documenti, seleziona la bozza e fai clic su &quot;Dettagli bozza&quot;. Si aprirà la scheda dei dettagli della bozza. Se la persona che desideri impostare come proprietario della bozza non è ancora presente nella bozza, puoi aggiungerla come destinatario facendo clic sul pulsante Idonei e selezionando Condividi. Una volta che la persona è stata aggiunta alla bozza (o se si trova già nella bozza), seleziona il pulsante Idonei corrispondente e fai clic su &quot;Rendi proprietario&quot;. Ora ne divengono i proprietari.

**domande**

Per quanto riguarda le nuove versioni delle bozze... l’unico modo comprensibile per farlo è trascinare e rilasciare il file sopra il file esistente. È questo il modo corretto di farlo?

**Risposta**

È consigliabile creare nuove versioni in questo modo: seleziona la bozza nella scheda Documenti, quindi fai clic sul pulsante Altro, scegli Nuova versione > Bozza. Viene visualizzata la pagina Nuova versione, che consente di trasferire il flusso di lavoro e di apportare le modifiche necessarie prima di distribuire la nuova versione.

**domande**

È possibile disabilitare i commenti sulle bozze per condividerle con un cliente in modo che non vedano tutti i feedback interni del team? In modo da non dover rigenerare una nuova bozza.

**Risposta**

È consigliabile utilizzare i modelli di flussi di lavoro automatizzati, che consentono di utilizzare &quot;Fasi private&quot;. Le fasi private consentono di nascondere i commenti, le annotazioni e le decisioni dei revisori ospiti in altre fasi. In questo modo, la revisione della bozza interna potrebbe essere completamente nascosta al richiedente esterno.

**domande**

La fase di bozza di Workfront viene aggiunta solo quando si utilizza l’utilizzo di flussi di lavoro automatizzati e qualcuno non aggiunto al flusso di lavoro apre la bozza?

**Risposta**

Se un non destinatario fa clic sulla bozza, viene aggiunta la fase &quot;Workfront Proof&quot; (Bozza di Windows) alle bozze. Verrà inoltre applicato se un utente converte una bozza del flusso di lavoro di base in una bozza di Automated Workfront.

**domande**

È possibile impostare un flusso di lavoro per la bozza in cui è possibile prendere più decisioni?

Stiamo cercando di fornire una segnalazione al nostro team legale interno su quando il consulente legale esterno ha completato le revisioni delle bozze (quanti giorni in media ci vogliono per completare la revisione, chi la completa, ecc.)

Abbiamo iniziato aggiungendo una nuova decisione al flusso di lavoro della bozza, denominata &quot;Revisione OC completata&quot;, e abbiamo pensato di poter creare un rapporto per tenere traccia di questi elementi.

Il problema è che sembra che si possa prendere una sola decisione sul flusso di lavoro.

**Risposta**

È possibile prendere più decisioni in merito a una bozza; tuttavia, sarà disponibile un solo stato generale per la bozza, che deriva dalla decisione relativa allo scenario peggiore sulla bozza, oppure dalla decisione presa da un’entità con potere decisionale primario.

A causa dei requisiti di reporting, ti consiglierei di fare in modo che tutti utilizzino le stesse opzioni di decisione (Approvato, Approvato con modifiche, Modifiche richieste), quindi di utilizzare i Rapporti nel Dashboard of Proof (Accesso PHQ > Rapporti) e di applicare l’opzione di filtro per filtrare in base ai destinatari (includi i destinatari del consulente legale esterno nel filtro). Potrai quindi visualizzare il tempo medio di rotazione delle bozze.

**domande**

Quando si trascina una nuova versione su una bozza esistente, perché TUTTI i ruoli cambiano o specificamente spariscono?

**Risposta**

Quando si trascina un documento come nuova versione, è corretto che il flusso di lavoro venga rimosso dalla nuova versione. Se desideri mantenere il flusso di lavoro dalla versione precedente alla versione successiva, seleziona la bozza nella scheda Documenti, quindi fai clic sul pulsante Altro, scegli Nuova versione > Bozza. Viene visualizzata la pagina Nuova versione, che consente di trasferire il flusso di lavoro e di apportare le modifiche necessarie prima di distribuire la nuova versione.

**domande**

Scenario - Inoltro delle bozze: un cliente esterno che rivede una bozza potrebbe voler circolare internamente nella sua organizzazione prima di approvare la bozza. Le altre revisioni non saranno necessariamente nel sistema, quindi non sembra che nei commenti funzioni @. Come dovrebbero condividere al meglio - inoltrare l’e-mail ed evidenziare al destinatario che eventuali commenti non verrebbero visualizzati come nome?

**Risposta**

Puoi utilizzare la funzionalità Sottoscrizioni bozze. Questo può essere abilitato nelle impostazioni della bozza e consente ai destinatari della bozza di inoltrare un collegamento pubblico generico alla bozza e quindi di consentire agli utenti di abbonarsi alla bozza (essenzialmente aggiungendo se stessi).

**domande**

Qual è la best practice per l&#39;utilizzo delle cartelle all&#39;interno dei documenti?

**Risposta**

Questo dipenderà dalla natura del progetto, ma è possibile considerare una cartella Bozze attive che contiene tutte le bozze/versioni attivamente instradate e una cartella Bozze approvate che contiene tutte le bozze finalizzate e approvate. Una volta approvata completamente una bozza, la si sposta dalla cartella Bozze attive alla cartella Bozze approvate.

**domande**

Se ho 3 persone in un gruppo di recensioni, posso impostare che ho bisogno di approvazioni da 2 di loro su 3?

**Risposta**

Sì.  Vorrai aggiungere le due persone per le quali hai bisogno di una decisione come revisori e approvatori e la terza persona come revisore.

**domande**

Inviare una bozza a un client esterno (utente non Workfront) per la revisione e i commenti. Vogliamo inviare loro una bozza pulita (in altre parole, senza commenti interni su di essa). Quali sono i passaggi corretti per garantire che il client esterno riceva la bozza (solo la bozza, nessun accesso al progetto stesso) e come fanno i client esterni a &quot;inviarci&quot; la loro bozza segnalata? Al momento non utilizziamo modelli di bozza/flussi di lavoro automatizzati.

**Risposta**

Per questo è consigliabile utilizzare modelli di flusso di lavoro automatizzato/flusso di lavoro automatizzato, in quanto consente di utilizzare la funzionalità &quot;Private Stage&quot;. Quando si utilizza la funzionalità Private Stage, è possibile che i commenti/le decisioni e i destinatari di determinate fasi della revisione rimangano nascosti alle persone in altre fasi. Ad esempio, potete avere uno stage interno come uno stage privato e uno stadio client. I client non saranno in grado di visualizzare nulla che abbia a che fare con lo stage interno, mentre l&#39;attività sarà visibile nello stage client.

**domande**

È possibile mantenere utenti specifici (come correttore di bozze) in una fase iniziale senza doverli collegare in fasi successive?

**Risposta**

Una volta che un utente viene aggiunto a una versione di una bozza in una fase, rimarrà su tale versione della bozza attraverso le fasi rimanenti. È possibile bloccare la fase successiva all&#39;inizio (o manualmente), in modo da impedire che sia possibile aggiungere ulteriori commenti.

**domande**

Dove è possibile visualizzare un elenco di tutti coloro che hanno rivisto e/o approvato una bozza, uno in quale giorno e a che ora? A fini di audit, ecc. Inoltre, esiste un luogo in cui è possibile visualizzare tutte le revisioni e le approvazioni per tutte le versioni di una bozza?

**Risposta**

Per visualizzare un elenco di attività, ad esempio quando sono stati effettuati commenti e decisioni, è necessario fare clic su nella Cronologia attività in Dettagli bozza. Per accedere a questa pagina, segui questo percorso: seleziona la bozza nella scheda Documenti > fai clic su Dettagli bozza > Espandi la sezione Attività. Se desideri visualizzare queste informazioni a livello di versione, segui questo percorso: seleziona la bozza nella scheda Documenti > fai clic sulla scheda Dettagli > Verso la parte inferiore dello schermo viene visualizzata la sezione Versioni. Da qui puoi accedere ai dettagli della bozza a livello di versione.

**domande**

Per favore, potete parlare un po&#39; di fasi private in prove.

**Risposta**

Quando una fase viene resa privata, i commenti e le decisioni non sono visibili agli utenti che non sono aggiunti a questa fase o che non sono supervisori, amministratori o amministratori di fatturazione nell’account. Inoltre, i revisori che vengono aggiunti a una fase privata possono vedere solo la fase a cui vengono aggiunti sulla bozza e i commenti fatti in quella fase.
