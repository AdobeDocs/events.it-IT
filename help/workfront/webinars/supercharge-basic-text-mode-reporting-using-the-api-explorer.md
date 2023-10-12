---
title: 'Domande all’esperto: creazione di rapporti in modalità testo di base con ricarica avanzata tramite API Explorer'
description: Scopri l’Explorer API, come utilizzarlo e come migliorare i rapporti sfruttando la modalità testo di base. Questo webinar è stato registrato il 22 gennaio 2020.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9918
exl-id: f859c4eb-8b3c-4d91-9765-9957dc4678f5
source-git-commit: 1792dc318643aec2c12613f621361d72a7a918b1
workflow-type: tm+mt
source-wordcount: '1662'
ht-degree: 2%

---

# Domande all’esperto: creazione di rapporti in modalità testo di base con ricarica avanzata tramite API Explorer

Scopri di più su [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/), come utilizzarlo e come migliorare i rapporti sfruttando la modalità di testo di base. Questo webinar è stato registrato il 22 gennaio 2020.

>[!VIDEO](https://video.tv.adobe.com/v/341124/?quality=12)

## Risorse aggiuntive

![Un grafico che mostra esempi di regole di codice in modalità testo](assets/text-mode-chart.png)


**Colonna finale &quot;Tutti i ruoli&quot;**

```
description="Primary =" indicates the user's primary job role
displayname=All Job Roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("Primary = ",{role}.{name}),{role}.{name})
valueformat=HTML
```

**Modalità testo per la colonna &quot;Tutti i team&quot;**

```
displayname=All Teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

**Modalità testo per la colonna &quot;Tutti i gruppi&quot;**

```
displayname=All Groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

**Modalità testo per colonna &quot;Report diretti&quot;**

```
displayname=Direct Reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

## Domande e risposte

**domande**

È possibile utilizzare una raccolta in un report utilizzando la modalità testo?

**Risposta**

Sì, è possibile utilizzare qualsiasi oggetto nell&#39;area delle raccolte. Desideri esplorare e vedere a cosa hai accesso. Non tutto avrà accesso sia all&#39;oggetto utente che all&#39;oggetto ruolo, come abbiamo visto con l&#39;oggetto Ruoli utente nell&#39;API Explorer.

**domande**

Puoi parlare di &quot;utilizzo condizionale di diverse raccolte nella stessa colonna (aggiornamenti di progetto e aggiornamenti delle attività)&quot;?

**Risposta**

Quando ci si trova nell&#39;area di iterazione e viene visualizzata l&#39;espressione valuefield o valueexpression, si accede a uno degli elementi dell&#39;elenco di raccolta. Utilizzando il campo valore è possibile ottenere il nome della mansione, ad esempio, o qualsiasi elemento presente in tale elemento dell’elenco. Se ci si trova in un&#39;attività, un oggetto attività può fare riferimento al progetto in cui si trova.

**domande**

Si può discutere se &quot;la raccolta di aggiornamenti delle attività è possibile solo in un report attività?&quot;

**Risposta**

Quando si crea un report sui problemi, è possibile visualizzare le informazioni sull&#39;attività se il problema è stato segnalato per l&#39;attività e tali informazioni potrebbero essere visualizzate anche dall&#39;interno della raccolta. Ad eccezione di quelle situazioni, per visualizzare i dati di raccolta delle attività è necessario essere in un report attività.

**domande**

È possibile condividere il formato testo ([!DNL CSS]) esempi?

**Risposta**

Workfront non supporta [!DNL CSS] in modalità testo.

**domande**

Qual è il modo migliore e/o più rapido per individuare un nome di campo personalizzato per il reporting in modalità testo? Ho usato l’opzione di modifica HTML nel browser OR aggiungendo un campo in un rapporto e passando alla modalità testo per afferrarlo MA... curioso di sapere come altri eseguono questa operazione

**Risposta**

Ho trovato più veloce per selezionare il campo nell&#39;interfaccia utente, quindi passare a Text Mode e copiare il nome del campo. In questo modo si ottiene l&#39;ortografia corretta per il campo.

**domande**

Come posso utilizzare la modalità testo per identificare i membri di un team in un rapporto? Attualmente usiamo le assegnazioni dei team nei flussi di lavoro di approvazione delle attività e vogliamo elencare i membri del team nella fase di approvazione corrente in una colonna simile a come funzionano i campi Approvatori e Stato.

**Risposta**

Per fare riferimento ai membri del team associati alla fase di approvazione corrente, è necessario fare riferimento a una raccolta di una raccolta a cui si fa riferimento, attualmente non possibile tramite le funzionalità della modalità testo di Workfront. La colonna attualmente in uso nell’organizzazione che mostra il team associato all’approvazione è l’opzione migliore.

**domande**

Il campo e il nome dell&#39;oggetto devono essere maiuscole/minuscole (ad es. ruolo e ruolo)?

**Risposta**

Quando fai riferimento a oggetti in modalità testo, vorrai scriverli esattamente come mostrato nella colonna di destra di API Explorer. Se ad esempio si desidera fare riferimento a un nome di progetto da un report attività, il campo valore sarà simile al seguente:

```
valuefield=project:name
```

Tuttavia, nel caso di Problemi, questi sono denominati opTasks in API Explorer. Pertanto, se desideri eseguire un rapporto sulle ore e aggiungere una colonna per il nome del problema, il campo del valore si presenterà come segue:

```
valuefield=opTask:name
```

**domande**

Sto cercando di creare un report che mostri per ogni progetto, le attività attive correnti su cui si sta lavorando. Come farei meglio a farlo? Immagino che sia un report di attività a cui sono state aggiunte anche colonne di informazioni sul progetto?

**Risposta**

È esatto. Un rapporto di attività è la soluzione migliore per questo. È necessario definire le &quot;Attività attive&quot;. Se si utilizzano i predecessori, si tratta di attività pronte. Quindi puoi filtrare per Ready = True. In questo modo verrebbero inserite tutte le attività pronte per l’avvio. È quindi consigliabile raggruppare le attività in base al nome del progetto, in modo da poter vedere immediatamente quali attività appartengono a ciascun progetto.

**domande**

Esiste un modo per creare rapporti che calcolano i dati, ad esempio % di progetti che soddisfano determinati criteri?

**Risposta**

Il modo migliore per creare un rapporto per presentare o calcolare i dati (ad esempio, %) consiste nell’applicare dei raggruppamenti al rapporto e quindi applicare un grafico. Se si desidera aggiungere un grafico a torta al report, è possibile impostare le sezioni della torta in valori o percentuali.

**domande**

È possibile utilizzare la modalità testo per identificare i membri di un team assegnati alla fase di approvazione dell&#39;attività corrente in modo simile alla colonna Approvatori e Stato?

**Risposta**

È necessario aggiungere una colonna della raccolta in modalità testo al report attività con le seguenti opzioni:

```
displayname=Current Approval Stage Approvers 
listdelimiter=<p> 
listmethod=nested(currentApprovalStep.stepApprovers).lists 
textmode=true
type=iterate 
valuefield=user:name 
valueformat=HTML
```

**domande**

È possibile filtrare la posizione in cui tutti i gruppi contengono un gruppo specifico?

**Risposta**

Se desideri filtrare gli elementi nel rapporto, puoi farlo nella scheda Filtro del rapporto. Pertanto, se desideri visualizzare solo gli utenti in cui uno dei loro gruppi era Contabilità, aggiungi una regola di filtro che dicesse:

```
Other Groups>ID>Equal>Accounting
```

**domande**

Esiste un modo per creare un rapporto che determini la durata effettiva di una combinazione di attività?

**Risposta**

È necessario filtrare il report in modo da includere solo la combinazione di attività desiderata. Successivamente, inserirai una colonna Durata effettiva nella vista e riepilogala in base alla Somma nelle Impostazioni colonna. Infine, dovrai raggruppare il report in un certo modo. Quando esegui il rapporto, la barra di raggruppamento mostra il totale delle durate effettive contenute nelle righe da raggruppare.

**domande**

Esiste un modo per sottrarre le attività che rientrano in un elemento padre per determinare la durata per il resto delle attività sotto un elemento padre?

**Risposta**

La durata di un&#39;attività padre viene calcolata sottraendo la data di inizio della prima attività iniziale dalla data di fine dell&#39;ultima attività padre. In un report si conoscono solo le singole attività che vengono prese in considerazione per la visualizzazione o meno. Il motore di report non ha modo di attenersi alle informazioni di un&#39;attività e utilizzarle quando si esamina un&#39;altra attività. Pertanto, l&#39;unico modo per eseguire la richiesta consiste nel rimuovere un&#39;attività da un determinato elemento padre nell&#39;elenco delle attività del progetto e osservare il ricalcolo della durata dell&#39;attività padre.

**domande**

Per i raggruppamenti condizionali, un modulo personalizzato (si pensi a &quot;Stati occidentali&quot;, &quot;Stati centrali&quot;, &quot;Stati orientali&quot;) per decodificare i singoli gruppi è una tecnica comune che funziona bene su quella nota, quando si consiglia di utilizzare i raggruppamenti calcolati rispetto ai parametri calcolati?

**Risposta**

I raggruppamenti calcolati (o espressione di valore in un raggruppamento) sono un modo pratico per ottenere un risultato da visualizzare nella barra dei raggruppamenti. Questa operazione può essere eseguita anche utilizzando un campo personalizzato calcolato. Per ogni approccio ci sono pro e contro, che sono:

* Le espressioni di valore vengono calcolate ogni volta che la pagina del browser viene aggiornata. Questo valore può essere migliore dei campi personalizzati calcolati che vengono ricalcolati ogni volta che l’oggetto a cui sono associati viene modificato, o quando i campi calcolati vengono ricalcolati in una modifica in blocco, o quando il modulo personalizzato viene modificato e l’opzione &quot;Aggiorna calcoli precedenti&quot; è selezionata.
* Tuttavia, le espressioni di valore non possono essere utilizzate nei grafici, nella formattazione condizionale o nel filtro. Per questi campi è necessario utilizzare campi personalizzati calcolati.

**domande**

Non è possibile cambiare il nome visualizzato del raggruppamento da &quot;No Value&quot; (Nessun valore) a qualcos’altro scelto per chiamarlo a scopo di reporting? In altre parole, sarà SEMPRE &quot;No Value&quot; (Nessun valore)?

**Risposta**

Esiste un modo per sostituire &quot;Nessun valore&quot; con qualcosa di diverso. Si supponga di avere un report di progetto raggruppato per nome Portfolio. Tutti i progetti non assegnati a un portfolio verranno raggruppati con il titolo:

```
Portfolio: Name: No Value
```

Per modificare questo valore, modifica il raggruppamento in modalità testo e sostituisci questa riga:

```
group.0.valuefield=portfolio:name
```

con questa riga:

```
group.0.valueexpression=IF(ISBLANK({portfolio}.{name}),"Not in any Portfolio",{portfolio}.{name})
```

Il raggruppamento avrà ora questo titolo:

```
Portfolio: Name: Not in any Portfolio
```

**domande**

Esiste un parametro per tenere traccia delle assegnazioni incomplete, ovvero:

1. Attività con una singola assegnazione a cui non è stato assegnato un utente singolo o
1. Attività con più assegnazioni a cui è stata revocata l&#39;assegnazione di almeno una persona per i ruoli richiesti

**Risposta**

Questo può essere fatto utilizzando un Rapporto di assegnazione e filtrando per

```
Assigned To ID > Is Blank and Role ID > Is Not Blank
```

Verranno incluse tutte le attività o i problemi assegnati a un ruolo, ma non necessariamente a un utente specifico. È necessario aggiungere le colonne per Attività e Nome problema per vedere a quale oggetto appartiene l’assegnazione e, se raggruppata per nome progetto, dovrebbe essere utile mantenerla organizzata.

**domande**

Chuck, mi dimentico, ma ricordi la proprietà in modalità testo che verrà poi riprodotta come descrizione, al passaggio del mouse?

**Risposta**

description= consente di visualizzare una descrizione comando quando si passa il puntatore sull&#39;intestazione di colonna.

**domande**

Posso creare un rapporto su un campo casella di controllo che consente selezioni multiple, ma solo estrarre la prima selezione nel rapporto?

**Risposta**

Sì.  Le scelte selezionate nel campo casella di controllo sono tutte in una stringa con ogni selezione separata da una virgola. Utilizzare l&#39;espressione SEARCH per trovare la posizione della prima virgola nel campo Casella di controllo, quindi utilizzare tale indice con l&#39;espressione LEFT per visualizzare il numero di caratteri dall&#39;inizio dell&#39;elenco. Ecco il codice:

```
valueexpression=IF(SEARCH(",",{DE:Checkbox Field},0)>0,LEFT({DE:Checkbox Field},SEARCH(",",{DE:Checkbox Field},0)),{DE:Checkbox Field})
```

Se utilizzi una virgola nel nome di una selezione nel campo della casella di controllo, la parte della selezione viene visualizzata solo fino alla prima virgola.
