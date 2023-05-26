---
title: 'Chiedi all’esperto: comprendere la combinazione e la capacità'
description: Scopri come misurare la combinazione e la capacità all’interno della tua azienda. Questo webinar è stato registrato il 2 ottobre 2019.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9913
exl-id: 5993c6c3-0583-4d1c-94aa-2e64a699e7f1
source-git-commit: ca06e5a8b1602a7bcfb83a43f529680a5a96bacf
workflow-type: tm+mt
source-wordcount: '2224'
ht-degree: 1%

---

# Chiedi all’esperto: comprendere la combinazione e la capacità

Scopri come misurare la combinazione e la capacità all’interno della tua azienda. Questo webinar è stato registrato il 2 ottobre 2019.

>[!VIDEO](https://video.tv.adobe.com/v/341119/?quality=12)

## Domande e risposte

**domande**

Come inserire %s in un istogramma?

**Risposta**

I valori % elencati nel rapporto Mix erano presenti perché nella scheda grafico sceglievamo &quot;Raggruppa colonne&quot; e &quot;Sovrapponi al 100%&quot;. Se scegliessimo &quot;In pila&quot;, mostrerebbe i totali delle ore pianificate e non la percentuale.

**domande**

Se il carico di lavoro di reparto/organizzazioni è una combinazione di progetti/attività e problemi/richieste, come consigliamo di ottenere una revisione di alto livello (in un rapporto Workfront) di un WPI.

**Risposta**

I progetti, le attività e i problemi devono disporre di propri report con i propri moduli personalizzati. Tuttavia, ciascuno di essi può utilizzare lo stesso campo Tipo di lavoro. Potrebbe essere necessario visualizzare i tre rapporti in un unico dashboard.

**domande**

È necessario modificare le attività in blocco per renderle operative o strategiche?

**Risposta**

La tecnica suggerita è quella di creare un rapporto che ti permetta di ottenere un elenco di attività operative. Dopo aver selezionato tutte le attività contemporaneamente, modificarle in blocco, quindi allegare il modulo personalizzato con Tipo di lavoro e impostare il tipo di lavoro su Operativo per tutte le attività contemporaneamente. Segui la stessa procedura per raccogliere un elenco di attività strategiche, modificarle in blocco e aggiungere il modulo personalizzato, ecc.

Nel webinar vengono menzionate alcune idee per prompt personalizzati che potrebbero aiutarti a ottenere un elenco, come verificare la presenza di determinate parole nel nome dell’attività, nel proprietario del progetto, nel portfolio o negli utenti assegnati. Queste sono solo idee. È necessario progettare un rapporto che funzioni al meglio nella propria situazione.

**domande**

Se nel mix sono presenti 4 categorie, è possibile creare un obiettivo per ogni categoria e quindi creare rapporti sui delta tra previsione e piano rispetto all&#39;effettivo? (4 categorie Campaign, Business Unit, Web e Product). A livello di progetto, le categorie sono disponibili nei campi o nei moduli personalizzati. L&#39;obiettivo consiste nel creare una previsione trimestrale (budget/previsione) e quindi nel tenere traccia delle ore pianificate in base a quella e alla fine effettive.

**Risposta**

Se hai tutte le categorie in un campo personalizzato (chiamiamolo per il momento Tipo di lavoro), crea un gruppo di report di progetto in base alle Ore pianificate, prima e Tipo di lavoro seconda. Filtra il report del progetto per visualizzare i progetti in Planning entro intervalli di date desiderati. Per visualizzare le percentuali, utilizzare un grafico con colonne o barre raggruppate sovrapposte al 100%. Questo potrebbe essere il rapporto Previsione.

Puoi copiare il rapporto e modificarlo per creare un rapporto basato sui progetti correnti, mostrando comunque il mix basato sulle ore pianificate.

Puoi copiare nuovamente il rapporto, impostarlo su Raggruppa per ore effettive invece che per ore pianificate e mostrare solo i progetti completati entro gli intervalli di date desiderati. Questo mostrerebbe il mix percentuale in base alle ore effettive.

**domande**

Funzionerà se disponi di diversi ID categoria per un progetto o un’attività?

**Risposta**

Sì, se disponi di più ID, questi devono essere separati da una scheda, come segue:

```
EXISTS:1:$$EXISTSMOD=NOTEXISTS
EXISTS:1:$$OBJCODE=OBJCAT
EXISTS:1:categoryID=5d76d82600e7926bb51eeb1e0886810e 5d54288d01034619f2eb2c74f6472f18
EXISTS:1:objID=FIELD:ID
```

Il modo migliore per separarli con un carattere di tabulazione è creare prima l’elenco delle categorie nel generatore. Inserisci più nomi di modulo personalizzati e quando passi alla modalità testo li visualizzerai come ID separati da tabulazioni.

Gli ID multipli vengono trattati come OR, quindi se uno di essi è allegato all’attività non verrà visualizzato nel rapporto.

**domande**

I prompt del report sono &quot;ANDed&quot; o &quot;ORed&quot;?

**Risposta**

I singoli prompt personalizzati sono &quot;ANDed&quot;. Pertanto, se si specifica Pam come proprietario del progetto e Bill come assegnato all&#39;attività, verranno visualizzate solo le attività assegnate a Bill che si trovano in progetti in cui Pam è il proprietario del progetto.

**domande**

Perché è possibile ordinare solo per determinate colonne? ovvero non è possibile ordinare per assegnazioni.

**Risposta**

&quot;Assegnazioni&quot; è un elenco e non è possibile ordinare o raggruppare in base a un elenco di elementi. È possibile ordinare o raggruppare solo un singolo elemento.

Per illustrare il punto, immagina un elenco di assegnazioni come questa su un&#39;attività:

```
Jane
Bill
Dan
```

E un elenco di assegnazioni come questa per un&#39;altra attività:

```
Bill
Jane
Helen
```

Quale attività deve essere visualizzata per prima in un ordinamento? Si potrebbe dire &quot;ordina in base al nome nell&#39;elenco&quot;, ma questo non è necessariamente utile, dal momento che non è possibile controllare l&#39;ordine. Workfront evita il problema non consentendo affatto l’ordinamento in base agli elenchi.

E il raggruppamento in base a un elenco? Se è possibile eseguire il raggruppamento in base a un elenco di nomi, tutte le attività assegnate a Jane, Bill, Dan verranno raggruppate e tutte le attività assegnate a Jane, Dan, Bill (lo stesso elenco, ma in un ordine diverso) verranno raggruppate in un raggruppamento diverso. Anche in questo caso, Workfront evita il problema non consentendo il raggruppamento per elenchi.

**domande**

Vengono utilizzate ore pianificate per attività strategiche e ore effettive per operazioni operative?

**Risposta**

No. Nel nostro esempio utilizziamo le ore pianificate per mostrare il livello di impegno pianificato sia per le attività strategiche che per quelle operative. Questo ci permette di confrontarli facilmente, sia nel passato, che nel presente o nel futuro. È inoltre possibile utilizzare le ore effettive per confrontare le attività strategiche e operative, ma solo per le attività passate, poiché le ore effettive sono quelle riportate dalle persone come tempo effettivamente dedicato alle attività.

**domande**

Nella pianificazione delle risorse, come vengono contabilizzate le attività pianificate in passato ma non completate? Le ore pianificate non sembrano essere riportate e pertanto non vengono visualizzate nelle settimane future come attività/ore che richiedono risorse.

**Risposta**

Non esiste un avanzamento &quot;automatico&quot; del lavoro non completato. In questo caso, dovrai ripianificare il progetto. È possibile che le risorse originariamente assegnate a una determinata attività non siano disponibili nel nuovo arco temporale, pertanto il project manager deve esaminare la questione e decidere il modo migliore per ripianificare. Ciò potrebbe comportare il coinvolgimento delle parti interessate e l&#39;ottenimento di approvazioni per le modifiche del piano.

**domande**

Invece di inserire 2 ore al giorno per controllare le e-mail, le interruzioni, consiglieresti di regolare il loro FTE?

**Risposta**

Sì, se si imposta l&#39;FTE su 0,75 per mostrare un utente disponibile 6 ore al giorno nella Programmazione delle risorse. Questa sarà la loro disponibilità ogni giorno. Se vuoi mostrarli come non disponibili per diversi periodi a seconda della data, ad esempio non disponibile l’ultimo giorno di ogni trimestre, puoi farlo con un progetto di costi comuni.

Alcune persone preferiscono i progetti di costi comuni perché possono costruirli per se stesse e modificarli quando lo desiderano, mentre potrebbero non avere i diritti per modificare il proprio FTE.

**domande**

I dati del dashboard capacità team sono disponibili per chiunque condivida il report, indipendentemente dalle autorizzazioni di cui dispone sul lavoro?

**Risposta**

Se un utente non dispone dell’autorizzazione per visualizzare l’oggetto, questo non sarà visibile all’interno del report/dashboard. Tuttavia, se desideri che tutti vedano gli stessi risultati, vai in Azioni rapporto > Modifica > Impostazioni rapporto e immetti nel tuo nome nel campo &quot;Esegui questo rapporto con i diritti di accesso di&quot;. In questo modo, gli utenti condivisi in questo report potranno vedere i risultati esatti visualizzati. Non concederà loro un accesso aggiuntivo al risultato stesso, quindi alcuni risultati possono essere cliccati o meno.

**domande**

Come è possibile creare un report che mostri tutto il personale assegnato a un progetto in generale (non a livello di attività)?

**Risposta**

È possibile creare una colonna all&#39;interno di un report di progetto che mostri tutti gli utenti elencati come parte della scheda Gestione del personale (Team di progetto). Utilizza la seguente modalità di testo:

```
displayname=Project Team
listdelimiter=<p>
listmethod=nested(projectUsers).lists
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

**domande**

Vorrei avere un rapporto/dashboard che incorpori il modo in cui funziona il mio team. In particolare, i seguenti scenari: - Progetti di mia proprietà / Progetti creati per me / Attività assegnate ad altri / Attività assegnate a me

**Risposta**

Progetti di mia proprietà

È disponibile un report integrato denominato &quot;Current Projects&quot; (Progetti correnti) che consente di visualizzare tutti i progetti correnti. Puoi modificare questo progetto e aggiungere una regola di filtro:Progetto > ID proprietario > Uguale a > $$USER.IDTon salvare e rinominare il report in &quot;Progetti di cui sono proprietario&quot;.

Progetti creati per me

È disponibile un report predefinito denominato &quot;I miei progetti&quot; che mostra tutti i progetti correnti presenti nel team del progetto (ovvero sei il proprietario, lo sponsor o l&#39;attività assegnata). Non sei sicuro di sapere se è quello che stai chiedendo, ma non ci sono altri modi per sapere se qualcuno ha creato un progetto per te, a parte quello di renderti il proprietario del progetto, di sponsorizzarti o di assegnarti un&#39;attività.

Attività che ho assegnato ad altri

Crea un rapporto di attività con i filtri desiderati, quindi passa alla scheda Filtro e fai clic su Passa a modalità testo. Aggiungi questo codice a qualsiasi elemento già presente:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Verranno visualizzate tutte le attività a cui l&#39;utente connesso ha assegnato almeno uno degli assegnatari correnti. Se gli assegnatari sono stati assegnati da più persone, nella pagina di destinazione dell’attività verrà visualizzato &quot;Richiesto da&quot; solo il nome della prima persona che ha assegnato qualcuno. Se desideri visualizzare tutte le persone assegnate a ciascuna di esse, puoi aggiungere una colonna alla vista, passare alla modalità testo e sostituire le eventuali colonne con quanto segue:

```
displayname=All Assignees and Requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

Attività assegnate a me

È disponibile un report predefinito denominato &quot;Le mie attività&quot; che mostra tutte le attività incomplete sui progetti correnti di cui sei il proprietario dell&#39;attività. Ti suggerisco di modificare il filtro per mostrare tutte le attività a cui sei uno dei potenzialmente molti utenti assegnati, non solo il proprietario dell’attività. Per farlo, rimuovi la regola del filtro

```
Task > Assigned To ID > Equal > $$USER.ID 
```

e la sua sostituzione con

```
Assignment Users > ID > Equal > $$USER.ID
```

**domande**

Esiste un modo per personalizzare le etichette nei grafici? Ho scoperto che quando creo un grafico per riflettere gli stati del progetto, il nome del gruppo predefinito viene incluso nell&#39;etichetta.

**Risposta**

Le etichette dei grafici utilizzano il nome del campo in base al quale si sta effettuando il raggruppamento. Pertanto, l’unico modo per modificare le etichette è utilizzare un campo personalizzato calcolato con qualsiasi nome desideri. Nella sezione di calcolo del campo, inserisci il nome del campo nativo in base al quale desideri eseguire il raggruppamento.

**domande**

Come si colorano le barre dei rapporti nelle assegnazioni del team di Chuck? Cioè ambra per dietro, rosso per tardi e verde per puntuale? È inoltre possibile modificare l’ordine in modo che sia più logico, ovvero rosso/ambra/verde o viceversa?

**Risposta**

Per modificare i colori utilizzati nel report per le opzioni Stato di avanzamento, modificare il report e fare clic sulla scheda Grafico. Cerca il menu a discesa &quot;Colori personalizzati >&quot;. Verrà visualizzato accanto alla casella &quot;Asse sinistro (Y)&quot; o alla casella &quot;Raggruppa dati per&quot;, a seconda che si scelga o meno di raggruppare colonne o barre. In tale elenco a discesa è possibile selezionare i colori. Se si fa clic sui numeri in basso a destra delle opzioni di colore, sarà possibile selezionare il colore da una pallette più grande.

Sfortunatamente non puoi modificare l’ordine di questi.

**domande**

È possibile creare un grafico che punti al numero di progetti in cui a un lavoratore viene assegnata un&#39;attività?

**Risposta**

Sì, ecco come:

* Creare un report di progetto
* Se l’utente in questione è l’utente connesso, il filtro deve includere questa riga:

```
   Project Users > ID > Equal >$$USER.ID 
```

* In caso contrario, sostituisci il nome utente con [!DNL $$USER.ID]. Verranno visualizzati tutti i progetti a cui questa persona è assegnata un&#39;attività oppure è il proprietario o lo sponsor. Se desideri visualizzare solo i progetti a cui sono state assegnate delle attività, aggiungi queste due regole di filtro aggiuntive:

```
   Project > Owner ID > Not Equal > $$USERID
   Project > Sponsor ID > Not Equal > $$USERID
```

* Creare almeno un raggruppamento per creare un grafico. Raggruppa tutto, come azienda. Fare quindi clic sulla scheda Grafico e scegliere un grafico. &quot;Conteggio record&quot; sarà l&#39;impostazione predefinita per un asse. Questo sarà il numero di progetti a cui l&#39;utente ha un&#39;assegnazione.

Quando a un utente viene assegnata un&#39;assegnazione in un progetto (assegnata a un&#39;attività, a un proprietario del progetto o allo sponsor del progetto), tale persona viene aggiunta al team del progetto e visualizzata nella scheda Gestione del personale della scheda secondaria Persone. Se un utente viene rimosso dall’incarico di proprietario del progetto, sponsor o con assegnazioni di attività, il suo nome rimane nel team del progetto. Deve essere rimossa manualmente se desideri rimuoverla. Tieni presente che questo potrebbe influire sulla precisione dei risultati del rapporto. Per rimuovere un utente dal team del progetto, passare a Personale > Persone, selezionare la persona o le persone desiderate, quindi fare clic sul pulsante Rimuovi visualizzato sopra l&#39;elenco.

**domande**

Come modificare l&#39;ordine decrescente di una colonna in modalità testo (in un raggruppamento)?

**Risposta**

È possibile scegliere di ordinare la maggior parte delle colonne nella scheda Colonne (Visualizzazione) durante la creazione di un report. Se non hai raggruppamenti, il rapporto dell’elenco verrà ordinato per intero. Se disponi di raggruppamenti, verrà ordinato in base a tale scelta all’interno di ciascun raggruppamento.

**domande**

Come si crea una colonna che identifichi i membri del team assegnati a una fase di approvazione?

**Risposta**

Se esegui un rapporto di attività o problemi/richieste, all’interno del Report Builder è disponibile una colonna denominata &quot;Approvatori e stato&quot; che raccoglierà queste informazioni.
