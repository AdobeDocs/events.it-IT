---
title: Ask the Expert - Qualità e coinvolgimento della misurazione
description: Scopri come creare rapporti che rispondono a domande su qualità e coinvolgimento. Questo webinar è stato registrato il 13 novembre 2019.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9914
exl-id: 76a8e418-71c7-414a-9938-e64e4e73c184
source-git-commit: 1792dc318643aec2c12613f621361d72a7a918b1
workflow-type: tm+mt
source-wordcount: '1211'
ht-degree: 1%

---

# Ask the Expert - Qualità e coinvolgimento della misurazione

Scopri come creare rapporti che rispondono a domande su qualità e coinvolgimento. Questo webinar è stato registrato il 13 novembre 2019.

>[!VIDEO](https://video.tv.adobe.com/v/341120/?quality=12)

## Domande e risposte

**domande**

Alcuni campi sono disponibili per il filtro ma non lo sono quando si tenta di raggrupparli in base a essi. Stai lavorando per renderle opzioni coerenti?

**Risposta**

Gli strumenti di reporting non consentono di raggruppare in base a un campo dinamico o a un campo che può avere più scelte selezionate contemporaneamente, come un campo casella di controllo. È possibile raggruppare solo i campi con un singolo valore, anche se possono avere molte scelte.

Puoi filtrare per caselle di controllo e visualizzarle, ma non puoi semplicemente raggrupparle.

**domande**

Nell’esempio di iterazione su mansioni, posso mostrare quella principale in grassetto?

**Risposta**

Nell’iterazione è possibile identificare il ruolo lavorativo principale. È necessario eseguire questa operazione in un’espressione di valore, ma i codici HTML non vengono riconosciuti in un’espressione di valore. Quindi dobbiamo trovare un altro modo per identificare il ruolo come primario. Ho inserito &quot;**&quot; prima e dopo il nome del ruolo principale in questo codice. Prova e scopri cosa ti piace:

```
displayname=All Job Roles 
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("**",{role}.{name},"**"),{role}. {name})
valueformat=HTML
```

Questo ti darà un elenco come questo:

```
Support Engineer 
QA Engineer 
**Designer**
```

Dove Designer è il ruolo principale per questo utente.

**domande**

Salve! Sto creando un flusso di lavoro per il nostro team editoriale che tiene traccia di dove si trova un articolo nel suo ciclo di vita (stesura iniziale —> recensioni reparto/i —> modifiche finali —> pubblicazione). Vogliono vedere facilmente a quale Milestone o Attività si trova attualmente. Il feedback che ricevo è che la vista Milestone standard (con l&#39;ombreggiatura rossa o verde) è troppo &quot;occupata e complessa&quot;. Esiste un modo per mostrare semplicemente &quot;Nome progetto&quot; e &quot;Cardine corrente&quot; in una tabella o griglia?

**Risposta**

Sì.  È possibile creare un report di attività che mostrerà le attività cardine su cui si sta lavorando e l&#39;attività a cui è associato. Puoi farlo in una tabella o in un rapporto elenco.

**domande**

È possibile combinare le informazioni della bozza con quelle del progetto in un rapporto?

**Risposta**

Se hai creato un rapporto Proof Approval (Approvazione della bozza), le informazioni del progetto possono essere inserite in colonne utilizzando la modalità testo. Ad esempio, se desideri fare riferimento al nome del progetto in una colonna, puoi utilizzare quanto segue:

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

**domande**

Vorrei anche maggiori informazioni sul reporting dei dati della bozza in relazione al progetto. Ad esempio, un rapporto di progetto che include la decisione relativa alla bozza e i commenti.

**Risposta**

Per fare riferimento alle informazioni sul progetto e sulla bozza in un unico rapporto, è necessario creare un rapporto Proof Approval (Approvazione della bozza). Attualmente, i commenti di una bozza non possono essere inseriti in questo report. Tuttavia, ogni decisione dell&#39;approvatore della bozza si trova sulla propria riga, nella colonna Decisione approvatore.

**domande**

Utilizzo spesso sharecol per creare lo stato di una singola pagina (molte colonne). Tuttavia, se dopo aver creato un rapporto voglio aggiungere una colonna nella parte superiore della pagina, tornare indietro e modificare richiede molto tempo. Hai suggerimenti o trucchi per effettuare questo tipo di modifica?

**Risposta**

Se si desidera inserire una colonna nella parte superiore di un elenco di colonne in modalità testo, sarà sufficiente rinumerare le colonne manualmente.

Tuttavia, se il rapporto è già stato creato e la prima colonna è costituita da colonne condivise e si desidera inserire un’altra colonna condivisa all’inizio dell’elenco, questa operazione risulta più semplice.

Nell’editor dei rapporti aggiungi solo un paio di nuove colonne e trascinale all’estrema sinistra della schermata Colonne (Visualizzazione). dopo aver eseguito questa operazione, osservare la colonna sinistra e i numeri di colonna in modalità testo sono stati tutti incrementati. Trascinare il numero di colonne vuote desiderato. Assicurati di inserire qualcosa in quelle colonne vuote prima di salvarla, altrimenti verranno rimosse.

**domande**

Ciao, per quanto riguarda il report finale sui bug, come si possono eseguire i report per più progetti, se sono in arrivo bug per più progetti??

**Risposta**

Puoi filtrare per portfolio o progetto, a seconda di come hai organizzato il tuo lavoro.

Puoi anche filtrare in base alle code di richieste. È possibile impostare code di richieste per ogni progetto in cui è possibile creare utenti cliente come revisori che possono accedere e inviare i ticket direttamente alle code di richieste condivise con loro.

**domande**

I primi rapporti erano basati sul nome dei progetti/progetti, questo può essere fatto anche sulle attività e, in caso affermativo, qual è il modo migliore per raggrupparle, dato che il nome dell’attività potrebbe essere diverso più spesso di quanto non lo sia...grazie!

**Risposta**

Tutte queste relazioni possono essere eseguite come relazioni su attività, problemi o progetti, a seconda di come si decide di tenere traccia degli elementi.

Un modo comune per raggruppare le attività consiste nel raggrupparle prima in base al nome del progetto e quindi in base al nome dell&#39;attività all&#39;interno di ciascun progetto. In questo modo, se si dispone di due attività con lo stesso nome, è facile vedere in quale progetto si trovano.

**domande**

Voglio sapere quali prove sono in sospeso, a quale attività e progetto sono legati, quando è stato instradato, quando è dovuto, e chi è il moderatore e l&#39;approvatore.

**Risposta**

Le bozze in sospeso possono essere filtrate da In attesa di decisione > È uguale a > True all’interno di un rapporto Proof Approval (Approvazione della bozza). È disponibile una colonna per l&#39;Approvatore che indicherà chi non ha ancora preso una decisione.

Puoi fare riferimento all’attività o al progetto a cui è associata la bozza utilizzando la modalità testo (vedi gli esempi di seguito).

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name
valueformat=HTML
```

Per quanto riguarda la data di instradamento, la data di scadenza e il moderatore, questi campi al momento non possono essere richiamati in nessuno dei rapporti di Workfront, pertanto dovrai fare clic direttamente nella bozza per visualizzare tali informazioni.

**domande**

È possibile impostare un modulo personalizzato da inviare automaticamente a un richiedente una volta completata la richiesta? Come un sondaggio sulla &quot;soddisfazione del cliente&quot;?

**Risposta**

Ecco una cosa che puoi fare che potrebbe soddisfare le tue esigenze. È possibile allegare una notifica di promemoria a un problema che invierà un messaggio e-mail a &quot;Inserito da&quot; dopo l’immissione di una data di completamento effettiva. L’Autore è la persona che ha creato il problema.

Puoi creare la notifica del promemoria, come abbiamo fatto nel webinar, per &quot;Promemoria per compilare la revisione dopo l’azione (AAR)&quot;, tranne per il fatto che si tratta di un promemoria relativo a un problema. Puoi anche creare un modello e-mail per il sondaggio. Dovrai applicare manualmente la notifica di promemoria a ogni problema (o utilizzare la modifica in blocco).

Un’integrazione sarebbe migliore in quanto potrebbe automatizzare i passaggi manuali, ma la notifica di promemoria può essere eseguita immediatamente.

**domande**

Ho creato un report che mostra i progetti per tipo di modello. Posso elencare il proprietario del progetto, ma non le persone assegnate a un progetto.

**Risposta**

Se si desidera richiamare il team del progetto (scheda Gestione del personale) in una colonna all&#39;interno del report del progetto, è necessario creare il team tramite la modalità testo. La modalità testo è la seguente:

```
displayname=Staffing 
listdelimiter=<p> 
listmethod=nested(projectUsers).lists 
textmode=true
type=iterate 
valuefield=user:name 
valueformat=HTML
```

## Codice modalità testo per il rapporto di coinvolgimento AAR

```
column.0.displayname=Task Details
column.0.value=<b>Project Name:</b>&nbsp;
column.0.valueformat=HTML
column.0.sharecol=true
column.1.valuefield=project:name
column.1.valueformat=HTML
column.1.sharecol=true
column.2.value=<br>
column.2.valueformat=HTML
column.2.sharecol=true
column.3.value=<b>Task Name:</b>&nbsp;
column.3.valueformat=HTML
column.3.sharecol=true
column.4.valuefield=name
column.4.valueformat=HTML
column.4.sharecol=true
column.5.value=<br>
column.5.valueformat=HTML
column.5.sharecol=true
column.6.value=<b>Task Owner:</b>&nbsp;
column.6.valueformat=HTML
column.6.sharecol=true
column.7.valuefield=assignedTo:name
column.7.valueformat=HTML
column.7.sharecol=true
column.8.value=<br>
column.8.valueformat=HTML
column.8.sharecol=true
column.9.value=<b>Actual Completion Date:</b>&nbsp;
column.9.valueformat=HTML
column.9.sharecol=true
column.10.valuefield=actualCompletionDate
column.10.valueformat=HTML
column.11.displayname=Name of Reviewer
column.11.linkedname=Name of Reviewer
column.11.namekey=view.relatedcolumn
column.11.namekeyargkey.0=Name of Reviewer
column.11.namekeyargkey.1=name
column.11.querysort=DE:Name of Reviewer:name
column.11.valuefield=Name of Reviewer:name
column.11.valueformat=customReferenceObjectAsString
column.12.displayname=AAR 1
column.12.description=In your view, does the work match stakeholders’ expectations? Did we achieve the intended results?
column.12.value=<b>AAR 1 Score:</b>&nbsp;
column.12.valueformat=HTML
column.12.sharecol=true
column.13.valuefield=AAR 1 - In your view, does the work match stakeholders’ expectations? Did we achieve the intended results?
column.13.valueformat=customDataLabelsAsString
column.13.sharecol=true
column.14.value=<br>
column.14.valueformat=HTML
column.14.sharecol=true
column.15.value=<br><b>AAR 1 User Comment:</b>&nbsp;
column.15.valueformat=HTML
column.15.sharecol=true
column.16.valuefield=AAR 1 User Comment
column.16.valueformat=customDataLabelsAsString
column.17.linkedname=direct
column.17.namekey=AAR 1 Reviewer Comment
column.17.querysort=DE:AAR 1 Reviewer Comment
column.17.valuefield=AAR 1 Reviewer Comment
column.17.valueformat=customDataLabelsAsString
column.18.linkedname=direct
column.18.displayname=AAR 1 Needs Attn
column.18.querysort=DE:AAR 1 Needs Attention
column.18.valuefield=AAR 1 Needs Attention
column.18.valueformat=customDataLabelsAsString
column.19.linkedname=direct
column.19.displayname=AAR 1 Needs Attn Notes
column.19.querysort=DE:AAR 1 Needs Attention Notes
column.19.valuefield=AAR 1 Needs Attention Notes
column.19.valueformat=customDataLabelsAsString
column.20.displayname=AAR 2
column.20.description=Do You Believe This Work Will Make an Impact?
column.20.value=<b>AAR 2 Score:</b>&nbsp;
column.20.valueformat=HTML
column.20.sharecol=true
column.21.valuefield=AAR 2 - Do You Believe This Work Will Make an Impact?
column.21.valueformat=customDataLabelsAsString
column.21.sharecol=true
column.22.value=<br>
column.22.valueformat=HTML
column.22.sharecol=true
column.23.value=<br><b>AAR 2 User Comment:</b>&nbsp;
column.23.valueformat=HTML
column.23.sharecol=true
column.24.valuefield=AAR 2 User Comment
column.24.valueformat=customDataLabelsAsString
column.25.linkedname=direct
column.25.namekey=AAR 2 Reviewer Comment
column.25.querysort=DE:AAR 2 Reviewer Comment
column.25.valuefield=AAR 2 Reviewer Comment
column.25.valueformat=customDataLabelsAsString
column.26.linkedname=direct
column.26.displayname=AAR 2 Needs Attn
column.26.querysort=DE:AAR 2 Needs Attention
column.26.valuefield=AAR 2 Needs Attention
column.26.valueformat=customDataLabelsAsString
column.27.linkedname=direct
column.27.displayname=AAR 2 Needs Attn Notes
column.27.querysort=DE:AAR 2 Needs Attention Notes
column.27.valuefield=AAR 2 Needs Attention Notes
column.27.valueformat=customDataLabelsAsString
column.28.displayname=AAR 3
column.28.description=Are you proud of the work you did on this?
column.28.value=<b>AAR 3 Score:</b>&nbsp;
column.28.valueformat=HTML
column.28.sharecol=true
column.29.valuefield=AAR 3 - Are you proud of the work you did on this?
column.29.valueformat=customDataLabelsAsString
column.29.sharecol=true
column.30.value=<br>
column.30.valueformat=HTML
column.30.sharecol=true
column.31.value=<br><b>AAR 3 User Comment:</b>&nbsp;
column.31.valueformat=HTML
column.31.sharecol=true
column.32.valuefield=AAR 3 User Comment
column.32.valueformat=customDataLabelsAsString
column.33.linkedname=direct
column.33.namekey=AAR 3 Reviewer Comment
column.33.querysort=DE:AAR 3 Reviewer Comment
column.33.valuefield=AAR 3 Reviewer Comment
column.33.valueformat=customDataLabelsAsString
column.34.linkedname=direct
column.34.displayname=AAR 3 Needs Attn
column.34.querysort=DE:AAR 3 Needs Attention
column.34.valuefield=AAR 3 Needs Attention
column.34.valueformat=customDataLabelsAsString
column.35.linkedname=direct
column.35.displayname=AAR 3 Needs Attn Notes
column.35.querysort=DE:AAR 3 Needs Attention Notes
column.35.valuefield=AAR 3 Needs Attention Notes
column.35.valueformat=customDataLabelsAsString
column.36.displayname=Done
column.36.valuefield=Review Complete
column.36.valueformat=customDataLabelsAsString
```
