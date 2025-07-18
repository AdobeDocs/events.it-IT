---
title: 'Chiedi all’esperto: misurazione della velocità'
description: Scopri come misurare e tenere traccia della velocità utilizzando il reporting  [!DNL Workfront] . Questo workshop è stato registrato il 14 agosto 2019.
doc-type: feature video
team: Technical Marketing
jira: KT-9912
last-substantial-update: 2023-08-15T00:00:00Z
exl-id: 83053de2-e386-4243-a9c8-a2ad9d51790f
duration: 4630
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '3962'
ht-degree: 0%

---

# Chiedi all’esperto: misurazione della velocità

Scopri come misurare e tenere traccia della velocità utilizzando il reporting [!DNL Workfront]. Questo workshop è stato registrato il 14 agosto 2019.

>[!VIDEO](https://video.tv.adobe.com/v/341057/?quality=12)

## Campi personalizzati utilizzati nella presentazione

Risparmia tempo copiando e incollando i calcoli di seguito.

>[!NOTE]
>
>La sintassi per i calcoli dei campi personalizzati è cambiata da quando la presentazione è stata data nel 2019, tuttavia i concetti e le altre istruzioni forniti nella presentazione sono ancora accurati.
>&#x200B;>**I calcoli inclusi di seguito sono stati aggiornati per riflettere le regole di sintassi più recenti.**

**Data primo commit**

Formato: Data

Calcolo:

```
IF(ISBLANK({DE:First Commit Date}),{defaultBaseline}.{plannedCompletionDate},{DE:First Commit Date})
```

**Prima Durata**

Formato: testo

Calcolo:

```
IF(ISBLANK({DE:First Duration}),{defaultBaseline}.{durationMinutes},{DE:First Duration})
```

**Proporzione lavoro-impegno**

Formato:Number

Calcolo:

```
ROUND(DIV({actualDurationMinutes},{DE:First Duration}),1)
```

**Stato rapporto lavoro su commit**

Formato:Text

Calcolo:

```
IF({DE:Work-to-Commit Ratio}>2,"Terrible",IF({DE:Work-to-Commit Ratio}>1.6,"Poor",IF({DE:Work-to-Commit Ratio}>1.2,"Not Bad","Excellent")))
```

**Velocità regolata**

Formato:Number

Calcolo:

```
ROUND(DIV({actualDurationMinutes},{durationMinutes}),1)
```

**Stato velocità regolato**

Formato:Text

Calcolo:

```
IF({DE:Adjusted Velocity}>2,"Terrible",IF({DE:Adjusted Velocity}>1.6,"Poor",IF({DE:Adjusted Velocity}>1.2,"Not Bad","Excellent")))
```

## Domande e risposte

**Domanda**

Ciao, grazie per aver organizzato questo webinar. Ho una domanda sul campo in Workfront. Nel nostro sistema, abbiamo creato un campo personalizzato denominato &quot;Stato&quot; che è una combinazione di Stato e Condizione. Questo campo State contiene molte statue in migliaia di progetti che è molto importante per il nostro estratto dati Tableau. Tuttavia, ora vogliamo eliminare questo campo e utilizzare il campo Condizione, il campo nativo. Hai idea di come posso capovolgere questo campo senza perdere dati. Tutto ciò che posso pensare di fare senza perdere dati in questo momento è cambiarlo manualmente da progetto a progetto.

**Risposta**

In una situazione come questa puoi utilizzare il filtro e la modifica in blocco per semi-automatizzare il processo di compilazione del campo Condizione in base al campo personalizzato Stato.

Di seguito sono riportati i passaggi da seguire:

1. Determinare quali valori di stato si desidera mappare ai valori di condizione. Ad esempio, supponiamo che tu abbia un valore di Stato &quot;Late&quot; (In ritardo) e &quot;Very Late&quot; (Molto in ritardo) entrambi mappati su un valore di Condizione &quot;In difficoltà&quot; (In Trouble)
1. Crea un report di progetti che mostra tutti i progetti con un valore di Stato &quot;In ritardo&quot; e &quot;Molto in ritardo&quot;
1. Esegui il rapporto. Assicurati di mostrare tutti i progetti (vedi le opzioni in basso a destra del rapporto)
1. Fai clic sulla casella di controllo in alto a sinistra del rapporto nella barra con le intestazioni di colonna. Verranno selezionati tutti i progetti nel rapporto
1. Fai clic sul pulsante Modifica sopra l’elenco dei rapporti
1. Impostare il tipo di condizione su Manuale
1. Imposta il campo Condizione su In difficoltà
1. Fai clic su Salva modifiche


**Domanda**

Come viene definito Excellent, Not Bad, etc (Eccellente, Non cattivo, ecc.)?

**Risposta**

Questo era solo un esempio, ma ecco come l&#39;ho impostato. Per prima cosa ho calcolato due indici:

Velocità regolata

La formula è Durata effettiva/Durata pianificata (memorizzata nel campo Durata in un progetto). Poiché la durata pianificata del progetto può cambiare ogni volta che il progetto viene ripianificato, la durata pianificata rappresenta la ripianificazione finale.

Proporzione lavoro-impegno

Questa formula è simile alla Velocità adeguata, con la differenza che invece di utilizzare il valore Durata pianificata della ripianificazione finale si desidera utilizzare la Durata pianificata promessa per la prima volta al cliente. Si presuppone che la baseline originale contenga queste informazioni (e da ora in poi si intende chiedere ai project manager di pianificare i progetti in modo da poter acquisire dati accurati). Abbiamo acquisito questo valore di durata dalla linea di base originale e lo abbiamo denominato Prima durata.

Dividendo la durata effettiva per la durata pianificata o per la prima durata si ottiene un numero che può dirci quanto siamo vicini a raggiungere l&#39;obiettivo. Se la durata pianificata o la prima durata è uguale alla durata effettiva, l’indice sarà uguale a 1. Se la durata effettiva è maggiore, la risposta sarà maggiore di 1. Maggiore è il numero peggiore che abbiamo fatto nel rispettare il nostro appuntamento.

Quindi, dato tutto ciò che ho deciso di assegnare gli stati sia per Velocità adattata che per Proporzione lavoro-impegno, nel modo seguente:

* 1.1 o inferiore ho chiamato Eccellente.
* Da 1.2 a 1.5 ho chiamato Not Bad.
* Da 1,6 a 1,9 ho chiamato Povero.
* 2 o più, ho chiamato Terribile.

**Domanda**

Cosa deve fare il lavoratore per tenere traccia del tempo necessario per eseguire i progetti?

**Risposta**

Qui non teniamo traccia delle ore effettivamente impiegate per i progetti, ma semplicemente monitoriamo e confrontiamo la durata. Ma se tieni traccia delle ore e desideri utilizzare le ore effettive sulle ore pianificate per calcolare la velocità, puoi fare lo stesso tipo di rapporto confrontando le ore pianificate con le ore effettive. Si desidera acquisire anche le ore pianificate dalla baseline originale.

**Domanda**

È possibile fornire i filtri utilizzati per Velocity?

**Risposta**

Ho utilizzato due regole di filtro per i rapporti Velocity:

* Categorie >> ID >> Uguale >> Dati progetto WPI (modulo personalizzato contenente tutti i campi calcolati). Desidero visualizzare solo i progetti che utilizzano questo modulo personalizzato)
* Progetto >> Stato > Uguale a > Completo (voglio vedere solo i progetti completati perché hanno un valore Durata effettiva che rappresenta il tempo necessario per completare tutto). I progetti attuali non fornirebbero una durata effettiva precisa per il calcolo della velocità)

Ho anche aggiunto altri filtri per mantenere il mio rapporto sufficientemente piccolo da gestire per il webinar, ma nel tuo ambiente di produzione probabilmente vorrai visualizzare tutti i progetti con il modulo personalizzato WPI in un particolare periodo di tempo. Puoi filtrare in base alla data di completamento effettiva del progetto.

**Domanda**

Se copi un progetto, questo avrà le stesse linee di base nel nuovo progetto?

**Risposta**

No, le previsioni non sono incluse nel progetto copiato

**Domanda**

Per un processo di approvazione attività, puoi mostrarmi come creare un rapporto che fornisca un audit trail per attività in un progetto con un timestamp per ogni approvatore?

**Risposta**

Creare un rapporto di attività. Nella scheda Colonne (Visualizzazione) fare clic su Aggiungi colonna. Nella casella &quot;Mostra in questa colonna:&quot; digitare &quot;approv&quot;. Verranno visualizzati i vari campi di approvazione disponibili per la generazione del rapporto. Suggerirei di aggiungere una colonna per tutto in un primo momento (tranne eventuali ID), in modo da poter vedere quali informazioni vengono visualizzate.

Quindi, passa alla scheda Filtri e aggiungi una regola di filtro per:

Task >> Is Approval (Approvazione) >> Equal (Uguale) > True (Vero). Verranno visualizzate solo le attività a cui è associata un&#39;approvazione.

Se necessario, aggiungi altri filtri.

**Domanda**

Vorrei creare un rapporto sulla bozza. Un elenco di progetti che mostra quante bozze hanno e quante versioni esistono.

**Risposta**

Crea un report documento.

Nella visualizzazione predefinita viene visualizzato il numero di versione. È possibile lasciare questo elemento in tale posizione, ma è possibile modificare qualsiasi altra colonna.

Raggruppa il report per nome progetto.

Il filtro del report per ID versione corrente:Proof non è vuoto.

Questo ti fornirà un elenco di tutte le bozze in ciascun progetto. Avrà una riga per ogni bozza e visualizzerà il numero di versione (che sarà uguale al numero totale di versioni).

**Domanda**

È possibile utilizzare la velocità a livello di attività? Piuttosto che a livello di progetto?

**Risposta**

Sì, ma dovrai copiare il modulo personalizzato del progetto e creare un modulo personalizzato per le attività da esso. Sarà quindi necessario modificare il calcolo nel campo Data primo commit e cambiare il riferimento a &quot;Previsione predefinita&quot; in &quot;Attività prevista predefinita&quot;. Fate lo stesso per la prima durata. In seguito è possibile allegare il modulo personalizzato dell&#39;attività a tutte le attività che si desidera misurare. Sarà necessario creare relazioni sulle attività invece di relazioni sui progetti per queste. Tuttavia, sarà comunque necessario assicurarsi che la baseline del progetto originale sia impostata come baseline predefinita. Tutti i dati dell&#39;attività vengono mantenuti nella stessa previsione con i dati del progetto.

**Domanda**

La data del primo commit deve essere impostata manualmente dal proprietario del progetto? Oppure può richiamare da campi esistenti?

**Risposta**

La data del primo commit viene acquisita dalla baseline predefinita. Se la previsione predefinita è quella originale, verrà visualizzata la data di completamento pianificata del progetto al momento in cui è stato impostato per la prima volta sullo stato Corrente.

**Domanda**

I campi calcolati nei moduli personalizzati devono ancora essere aggiornati periodicamente e corretti? Oppure accadrà automaticamente durante la notte (o in un altro momento)?

**Risposta**

I campi calcolati vengono ricalcolati:

* Quando un utente modifica l’oggetto
* In caso di modifica in blocco con le espressioni personalizzate ricalcolate attivate
* Modifiche al modulo con l’opzione &quot;Aggiorna calcoli precedenti&quot; selezionata

**Domanda**

Se la velocità considera la durata, la percentuale di completamento nella preferenza progetto deve essere basata sulla durata?

**Risposta**

No, l&#39;opzione Preferenze progetto si riferisce solo alla modalità di calcolo della percentuale di completamento. Questa impostazione non influisce sul valore della durata stessa.

**Domanda**

Qual è la differenza tra la durata del primo piano e quella del piano?

**Risposta**

Prima durata è il numero di giorni promessi originariamente al cliente per il progetto. Questo numero viene ottenuto dalla previsione originale registrata quando il progetto è stato cambiato da Pianificazione a Corrente.

Durata pianificata è il numero di giorni dall&#39;inizio del progetto alla Data di completamento pianificata. Inizialmente queste due durate sono le stesse, ma se il progetto è stato ripianificato e la Data di completamento pianificata è stata modificata, anche la Durata pianificata è stata modificata.

Il valore dei rapporti Velocity deriva dalla possibilità di vedere quanto è cambiata la durata pianificata rispetto alla prima durata. È possibile vedere questo dato già all&#39;inizio della registrazione delle previsioni quando i progetti sono cambiati da Pianificazione a Attuale.

**Domanda**

È possibile impostare i processi di lavoro in base al colore in modo che siano uguali in tutti i rapporti?

**Risposta**

Se si raggruppa per Assegnato a >> Nome in un report attività, è possibile assegnare un colore a determinati lavoratori nella scheda Grafico. È sufficiente scegliere l&#39;opzione Colori personalizzati accanto alla casella Assegnato a >> Nome nella scheda Grafico e aggiungere un colore per ogni lavoratore.

**Domanda**

Si sta tentando di determinare se è possibile creare un dashboard con un&#39;area che esamina un modulo personalizzato a livello di attività per verificare se è presente e secondario se alcuni campi non sono vuoti. È possibile?

**Risposta**

Vediamo se capisco la tua domanda. Si supponga di disporre di un modulo personalizzato per le attività denominato Modulo Tammy con un campo denominato Campo Tammy.

Si desidera creare un report delle attività che mostri tutte le attività a cui è allegato il modulo Tammy e in cui il campo Tammy contiene un valore.

Sì, puoi farlo. Dovresti semplicemente disporre di un filtro nel rapporto attività con due regole di filtro:

Categorie >> Modulo ID Equal Tammy

Task >> Il Campo Tammy Non È Vuoto

**Domanda**

È possibile creare un report per cercare un documento con nome specifico nella raccolta documenti? Parte del dashboard che vogliamo misurare se esistono determinati documenti.

**Risposta**

Sì.  È necessario creare un report Documento. Potrebbe essere necessario specificare un nome specifico per il documento ogni volta che si esegue il report. In questo caso, consiglierei di passare a Opzioni rapporto e selezionare Prompt rapporto. Aggiungi un prompt per Documento >> Nome.

**Domanda**

È possibile scegliere un colore o un valore esadecimale non elencato nella scheda del grafico, ma che sia un nuovo colore, ovvero un nuovo valore esadecimale, ad esempio un nuovo colore dei colori del mio marchio per consentire la personalizzazione dei rapporti?

**Risposta**

Sì, puoi immettere qualsiasi codice RGB che potresti essere stato in grado di trovare. Si tratta di un codice standard che indica la quantità di rosso, verde e blu contenuta nel colore. Workfront accetterà qualsiasi valore esadecimale da 000000 a FFFFFF, quindi se conosci il codice del colore del tuo marchio puoi utilizzarlo.

**Domanda**

È possibile riaffermare la definizione dei rapporti nel dashboard (fornire una dichiarazione di ciò che ogni rapporto misura)?

**Risposta**

Grafico di stato della velocità regolata

> Questo mostra quanto siamo riusciti a completare i progetti in tempo quando abbiamo confrontato la durata effettiva del progetto con la durata pianificata. La durata pianificata è stata adeguata in quanto il progetto è stato ripianificato durante il suo ciclo di vita.

Grafico stato rapporto lavoro-commit

> Questo mostra quanto siamo riusciti a completare i progetti in tempo quando abbiamo confrontato la durata effettiva del progetto con la prima durata. La prima durata era l’ora originale per la quale promettevamo al cliente che il progetto sarebbe stato completato. La prima durata è stata calcolata dal valore Durata del progetto quando è stato modificato per la prima volta dallo stato Pianificazione allo stato Corrente. Questa era la durata registrata nella linea di base Originale.

Rapporto Elenco stato velocità

> Questo rapporto contiene tutti i campi personalizzati calcolati e le date significative per gli stessi progetti nei grafici. Il suo scopo è quello di consentirci di controllare i nostri calcoli e ottenere informazioni più dettagliate, se desiderato.

**Domanda**

Come hai aggiunto i nuovi dati all’asse x?

**Risposta**

Quando si esegue il raggruppamento in base a qualsiasi elemento in un report, è possibile creare un grafico. È quindi possibile impostare l&#39;asse X o Y nella scheda Grafico.

**Domanda**

Puoi analizzare la differenza tra la prima durata e la durata effettiva?

**Risposta**

Prima durata è il numero di giorni promessi originariamente al cliente per il progetto. Questo numero viene ottenuto dalla previsione originale registrata quando il progetto è stato cambiato da Pianificazione a Corrente.

Durata effettiva è il numero di giorni compresi tra l&#39;inizio del progetto e la data di completamento effettiva.

**Domanda**

Come si inserisce il fattore di previsione del progetto in questo rapporto?

**Risposta**

La previsione originale del progetto contiene la data di completamento pianificata e la durata pianificata che esistevano quando il progetto è stato modificato per la prima volta nello stato Attuale. Se il processo deve pianificare il progetto prima di impostarlo su Corrente, verrà indicata la data entro la quale si è impegnato a completare il progetto.

**Domanda**

Esiste un modo per applicare in massa il nuovo modulo ai vecchi progetti?

**Risposta**

Sì, è possibile selezionare più progetti da un elenco. In questo caso, nella parte superiore sinistra dell&#39;elenco viene visualizzata l&#39;opzione &quot;Modifica&quot;. Quando si selezionano più oggetti e si fa clic su Modifica, si entra in quella che viene chiamata &quot;modifica in serie&quot;. Puoi aggiungere un modulo personalizzato a più progetti in questo modo.

Per aggiungere moduli personalizzati a un numero elevato di progetti, è possibile creare un rapporto filtrato in modo da includere solo i progetti desiderati. Quindi, invece di selezionare i progetti singolarmente, fai clic sulla casella di controllo sopra la prima casella nell’elenco e selezionerai l’intero elenco.

**Domanda**

È possibile rimuovere le voci duplicate dall&#39;interno del raggruppamento in un report di assegnazione, ma non tra raggruppamenti?

**Risposta**

Il modo migliore per pensare ai raggruppamenti nei rapporti sugli elenchi è questo:

Innanzitutto, puoi controllare gli elementi da visualizzare nell’elenco utilizzando la scheda Filtro. Non ci saranno voci duplicate. Il filtro viene applicato a ogni oggetto. Se passa attraverso il filtro, verrà visualizzato una volta nell’elenco, altrimenti non verrà visualizzato affatto.

Il raggruppamento successivo viene applicato all’elenco filtrato. Un raggruppamento identifica una cosa sugli oggetti dell’elenco, come il nome del portfolio in cui si trova (non è possibile eseguire il raggruppamento in base a un elenco di elementi, ma solo in base a un singolo elemento). Quindi tutti gli oggetti con lo stesso valore appariranno in quel raggruppamento, come tutti i progetti nello stesso portfolio. Tutti i progetti per i quali non è selezionato un portfolio vengono visualizzati nel raggruppamento denominato &quot;No Value&quot; (Nessun valore).

Di conseguenza, nessun oggetto può essere visualizzato in più raggruppamenti. La visualizzazione di un oggetto nell&#39;elenco è completamente controllata dal filtro e dalla persona che esegue il report dispone dei diritti per visualizzarlo.

**Domanda**

Consiglieresti altri rapporti per tenere traccia di Velocity? Solo una raccomandazione di alto livello è grande perché so che non c&#39;è abbastanza tempo per passare attraverso i dettagli.

**Risposta**

Come per qualsiasi rapporto, la prima cosa da fare è decidere cosa si desidera sapere. Il passaggio successivo consiste nell’accedere a tali informazioni, il che in alcuni casi significa che devi iniziare a tracciarle.

Una ragione per cui ho deciso di confrontare la Durata Reale con due tipi di Durata Pianificata è perché ho pensato che fornisse informazioni interessanti sulla velocità. Anche i dati erano già disponibili, quindi non dovevo iniziare a tracciarli. Con alcuni calcoli, potevo estrarre i dati in un modulo e creare un report.

È tuttavia possibile decidere di tenere traccia di altre informazioni relative ad attività o progetti da includere nei rapporti.

Workfront non ha alcun rapporto integrato sulla velocità; pertanto, ti consiglierei di fare un brainstorming con il tuo team per capire cosa vuoi sapere per determinare la velocità e capire cosa devi tracciare.

**Domanda**

È possibile calcolare qualcosa a livello di COLONNA? Invece di chiamare un CAMPO calcolato da un modulo personalizzato?

**Risposta**

Per eseguire questi calcoli, sarebbe stato possibile utilizzare un’espressione di valore in modalità testo. Tuttavia, non avremmo potuto eseguire la prima durata o la prima data di impegno, avevamo bisogno di catturarli in un luogo in cui non sarebbero cambiati.

Per quanto riguarda lo stato del rapporto tra lavoro e impegno e lo stato della velocità adeguato, questi dovevano essere campi personalizzati in modo da poterli utilizzare nella scheda Grafico. La scheda Grafico non riconosce i raggruppamenti in modalità testo, devono essere campi personalizzati. E siccome avevamo bisogno di Work-to-Commit Ratio (Rapporto lavoro-impegno) e di Adjusted Velocity (Velocità adattata) per calcolare quegli stati, avevamo bisogno che fossero anche campi personalizzati. In questo caso dovevano essere tutti campi personalizzati, ma è sempre bene considerare entrambi i modi e scegliere quello che funzionerà meglio. Grazie per la domanda.

**Domanda**

I nostri progetti cambiano spesso a causa di ritardi o modifiche dei clienti durante il processo. La nostra relazione potrebbe essere &quot;terribile&quot;. Cosa si consiglia di fare per tenere traccia dei motivi delle modifiche? Abbiamo pensato di aggiungere un modulo personalizzato a livello di documento che segnala il motivo della modifica (interna o client), ma ci chiediamo quale sia la best practice.

**Risposta**

La best practice consiste nell’utilizzare un elenco a discesa per tenere traccia di questo elemento. Inserisci il maggior numero di &quot;ragioni&quot; possibile in per iniziare, quindi aggiungi un’opzione &quot;altro&quot; per acquisire un motivo non presente nell’elenco. Se il nuovo motivo si presenta o diventa comune, aggiungilo al menu a discesa. È possibile creare report sugli elementi di un elenco a discesa e raggruppare in base a questo campo, ma non in base alle caselle di controllo o a un elenco a discesa a selezione multipla.

Solo un altro commento. Potrebbe non essere necessario includere tutti i progetti nei rapporti Velocity. Se stai correggendo bug o &quot;andando dove nessuno è andato prima&quot; probabilmente non stai assumendo lo stesso tipo di impegno per una data di completamento come se si stesse costruendo una casa che hai costruito molte volte in precedenza.

Assicurati quindi di concentrare il reporting sulla velocità sui punti in cui può aiutarti a raggiungere i tuoi obiettivi.

**Domanda**

Se si imposta la previsione predefinita su &#39;Originale&#39; per un progetto, quindi si riposiziona il progetto fuori dal progetto corrente, verrà modificata la previsione predefinita?

**Risposta**

Sì.  Ogni volta che si cambia lo stato in Corrente, viene creata una nuova linea di base, che sarà quella predefinita. Tuttavia, tutte le baseline precedenti esisteranno ancora e sarà possibile impostare manualmente la baseline originale come predefinita.

**Domanda**

Esiste un modo per impostare in un rapporto quali campi sono modificabili? È possibile impostare restrizioni per determinati campi?

**Risposta**

È possibile limitare i diritti di visualizzazione e modifica per i campi di un modulo personalizzato. È necessario includere i campi in una sezione e nelle impostazioni della sezione è possibile scegliere i diritti necessari per consentire agli utenti di visualizzare o modificare i campi nella sezione.

**Domanda**

È possibile creare un report che cerchi un documento con nome specifico nella raccolta documenti?

**Risposta**

Sì.  È necessario creare un report Documento. Potrebbe essere necessario specificare un nome specifico per il documento ogni volta che si esegue il report. In questo caso, consiglierei di passare a Opzioni rapporto e selezionare Prompt rapporto. Aggiungi un prompt per Documento >> Nome.

**Domanda**

Nei rapporti, perché i valori sono disponibili come colonna ma non per la selezione o il raggruppamento? Ad esempio: Issue Source.

**Risposta**

Il motivo principale per cui una colonna potrebbe essere visualizzabile ma non disponibile per il raggruppamento è che potrebbe contenere un elenco, ad esempio caselle di controllo, campi personalizzati o assegnazioni di attività. Il raggruppamento in un elenco non è consentito.

**Domanda**

Come posso separare in un rapporto (in base a quali campi) quando è avvenuta l’immissione di ore e quando le ore sono state effettivamente eseguite?

**Risposta**

Il campo Data immissione per l&#39;oggetto Hour si riferisce alla data di lavoro delle ore. In questo modo la Data di ingresso è diversa da quella di altri oggetti, dove indica la data di creazione dell&#39;oggetto. Anche se non esiste una data di creazione per le ore, esiste una &quot;Data ultimo aggiornamento&quot;, che è inizialmente la data di creazione e poi qualsiasi data in cui l’ora è stata modificata successivamente.

**Domanda**

Dal punto di vista della generazione rapporti, come possiamo accedere ai dati della linea di base? Ho un progetto con più linee di base. Desidero vedere come sono state pianificate le singole attività in ogni previsione. Esiste un modo per scrivere un report che mostri il piano del progetto per ogni previsione?

**Risposta**

In un report verranno visualizzati i campi che si desidera visualizzare per la baseline attualmente impostata come predefinita, in modo da poter modificare la baseline e aggiornare il report per visualizzare i campi con la nuova baseline.

Tuttavia, se si desidera visualizzare graficamente le informazioni sulle attività, è possibile farlo utilizzando la funzione del diagramma di Gantt. Attiva Gantt in un elenco di attività (utilizzando l’icona Gantt in alto a destra accanto a Salvataggio automatico), passa all’icona Impostazioni appena sotto e a destra e fai clic su di essa. Selezionare la casella Baseline per visualizzare tutte le baseline. È possibile selezionarli uno alla volta e visualizzare le modifiche apportate alle attività nella visualizzazione Gantt.

**Domanda**

Come creare un report per trovare le modifiche nel relativo stato per un periodo definito, ad esempio il mese scorso.

**Risposta**

La funzione Analytics di Workfront consente di visualizzare i dati storici, comprese le modifiche di stato.

È tuttavia possibile ottenere informazioni sulla modifica dello stato utilizzando un report Nota. È possibile filtrare per visualizzare le modifiche di stato sui progetti se si tiene traccia del campo Stato progetto.

Quindi prima, vai a Configurazione>Interfaccia>Feed di aggiornamento e assicurati che lo Stato del progetto sia uno dei Campi incorporati che vengono tracciati. Se non lo è, devi aggiungerlo.

Ora crea un rapporto di nota ed effettua le seguenti operazioni:

Nella scheda Colonne (Visualizza):

* Sostituire la colonna &quot;Testo nota&quot; con &quot;Testo di controllo&quot;. Verranno visualizzate informazioni sulle modifiche apportate allo stato da e a
* Lascia le colonne &quot;Progetto: Nome&quot; e &quot;Data di ingresso&quot;
* Fate clic sulla colonna &quot;Data di ingresso&quot;, quindi selezionate &quot;Ordina per questa colonna&quot; nel pannello Impostazioni colonna. Se desideri visualizzare le modifiche di stato più recenti in alto, ordinale in modo decrescente.

Nella scheda Raggruppamenti:

* Raggruppa per progetto: Nome

Nella scheda Filtri, crea le seguenti regole di filtro:

* Nota >> Tipo di controllo >> Uguale a >> Modifica stato
* aggiungi eventuali regole aggiuntive da filtrare in base alla data di immissione della nota. Puoi scegliere di escludere questo valore da Filtri e di utilizzare al suo posto un prompt per report
* Puoi filtrare in base al progetto, al portfolio o ad altri dati.

**Domanda**

Come Planner puoi richiamare rapporti per altri utenti?

**Risposta**

Un planner può creare rapporti e condividerli con qualsiasi utente, anche con persone che non sono utenti. Quando visualizzi il rapporto, passa a Azioni rapporto>Condivisione, quindi fai clic sull’icona a forma di ingranaggio in alto a destra nella casella Accesso ai rapporti. Scegli &quot;Rendi pubblico per gli utenti esterni&quot;. opzione. Puoi copiare il collegamento fornito e inviarlo a chiunque. Il rapporto verrà visualizzato in tempo reale nel browser.
