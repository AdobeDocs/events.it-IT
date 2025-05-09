---
title: Mastering della logica sequenziale in Adobe Analytics e Customer Journey Analytics - Avvio e arresto
description: Padroneggia la logica sequenziale in Adobe Analytics con segmentazione avanzata, controlli dell’ambito e campi derivati per scoprire i modelli di comportamento dei clienti e migliorare l’accuratezza dei dati.
solution: Analytics, Customer Journey Analytics
role: Developer
level: Intermediate
doc-type: Event
duration: 3370
last-substantial-update: 2025-05-08T00:00:00Z
jira: KT-18017
source-git-commit: cfc7b54ae4360779ca2c41f88fc08089bae99165
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---


# Mastering della logica sequenziale in Adobe Analytics e Customer Journey Analytics: avvio e arresto

In questa sessione esamineremo come configurare le sequenze con l’operatore THEN in Adobe Analytics (AA) e Customer Journey Analytics (CJA). Scopri come recuperare sottoinsiemi precisi di attività combinando SOLO DOPO/SOLO PRIMA DELLA SEQUENZA con i punti di controllo EXCLUDE.

## Punti di discussione

* Revisione rapida degli operatori logici sequenziali autonomi e del framework visivo.
* Descrivere in che modo l&#39;opzione ESCLUDI influisce sui risultati delle sequenze utilizzando SOLO SEQUENZA DOPO/PRIMA.
* Casi d’uso e demo attuali che mostrano come puoi adottare i metodi per la tua azienda.

>[!VIDEO](https://video.tv.adobe.com/v/3458040/?learn=on&enablevpops)

## In evidenza


1. Logica sequenziale e segmentazione in Analytics

   * La sessione si è concentrata su tecniche avanzate per applicare la logica sequenziale nell’analisi, sottolineando l’importanza di comprendere i punti di inizio e di fine nelle sequenze di dati per analizzare in modo efficace i comportamenti dei clienti.
   * Gli operatori sequenziali sono stati discussi come strumenti per identificare pattern quali &quot;hit web seguito da hit e-mail&quot; o &quot;invio di applicazioni seguito da sessioni successive&quot;.
   * È stata evidenziata la natura greedy della logica dei segmenti, che spiega come restituisce il set di dati più grande possibile a meno che non sia vincolata da condizioni aggiuntive.
   * Sono state introdotte tecniche per definire l’ambito, come sequenze &quot;solo prima&quot; e &quot;solo dopo&quot;, per studiare sottoinsiemi di dati in base a specifiche domande di business.
   * L’utilizzo di punti di controllo, condizioni di prossimità e criteri di esclusione è stato spiegato per perfezionare l’analisi dei dati e rispondere a domande di business complesse.

2. Gestione di più punti di interesse nell’analisi dei dati

   * Andy ha discusso gli scenari in cui i clienti hanno più richieste di applicazioni e la necessità di analizzare i comportamenti dopo ogni richiesta, anziché solo la prima.
   * Sono state affrontate sfide quali la sovrapposizione delle richieste e la definizione dell’inclusione o esclusione dei punti di interesse originali.
   * È stata sottolineata l’importanza di chiarire le ipotesi e perfezionare la logica per gestire più occorrenze di una sequenza, garantendo un’analisi accurata dei comportamenti dei clienti durante il loro ciclo di vita.

3. Tecniche avanzate per interrompere la corrispondenza dei dati

   * La sessione ha introdotto metodi per interrompere la corrispondenza dei dati in punti di controllo specifici utilizzando criteri di esclusione, consentendo agli analisti di studiare i dati tra punti di inizio e punti di arresto definiti.
   * Alcuni esempi includono l’analisi dei comportamenti tra &quot;hit web seguito da interazione con app mobile&quot; e l’arresto in &quot;interazione e-mail&quot;.
   * L&#39;uso di condizioni &quot;dentro&quot; e &quot;dopo&quot; è stato spiegato per applicare regole di prossimità più severe ed evitare risultati indesiderati da una logica avida.
   * Andy ha dimostrato come queste tecniche possono essere applicate per studiare i comportamenti dei clienti relativi a eventi specifici, come l’invio di richieste.

4. Convalida e perfezionamento della logica di analisi dei dati

   * Andy ha sottolineato l’importanza di convalidare le ipotesi e testare la logica per garantire risultati accurati, in quanto gli errori nella creazione dei segmenti o le ipotesi di dati sono comuni.
   * Sono stati condivisi esempi di risultati inattesi dovuti a logiche avide, evidenziando la necessità di condizioni rigide come &quot;all&#39;interno di un evento&quot; o &quot;all&#39;interno di una sessione&quot;.
   * Per testare e perfezionare i metodi di analisi sono stati raccomandati parametri di riferimento di convalida, come piccoli set di dati con caratteristiche note.

5. Applicazione della logica sequenziale a casi d’uso reali

   * Andy ha fornito esempi di casi d’uso reali, come l’analisi del comportamento dei clienti dopo l’invio delle applicazioni o l’identificazione di azioni comuni a seguito di acquisti o recensioni negative.
   * La sessione ha dimostrato come la logica sequenziale possa essere applicata a modelli di studio come &quot;prima sessione dopo l&#39;applicazione&quot; o &quot;seconda sessione dopo l&#39;applicazione&quot; in più occorrenze.
   * È stata discussa l’importanza di scalare l’analisi per set di dati più ampi mantenendo al contempo l’accuratezza, con esempi di effetti a cascata nei dati a livello di sessione.

6. Utilizzo di campi derivati per analisi flessibili

   * Andy ha introdotto il concetto di utilizzo di campi derivati in Adobe Customer Journey Analytics (CJA) per definire dinamicamente i momenti di interesse, riducendo la necessità di modificare più filtri per ogni analisi.
   * I campi derivati consentono agli analisti di creare filtri relativi a un singolo campo, consentendo adeguamenti rapidi per studiare diversi punti di interesse, ad esempio applicazioni specifiche per il prodotto o altri eventi per i clienti.

7. Applicazioni pratiche e piani futuri

   * Andy ha condiviso i piani per la prossima sessione del webinar, che si concentrerà su modelli, schede di riferimento e applicazioni pratiche dei concetti discussi, passando dalla formazione ai casi d’uso utilizzabili.
   * La sessione si è conclusa con una richiesta di feedback tramite un sondaggio per determinare l&#39;interesse per gli argomenti futuri e garantire l&#39;allineamento con gli obiettivi dei partecipanti.
   * Andy ha evidenziato i micro-impegni del team Ultimate Success, offrendo sessioni di coaching mirate per aiutare le aziende ad applicare questi concetti ai loro casi d’uso specifici.

8. Condivisione di materiali e azioni di follow-up

   * Andy ha confermato che il materiale del webinar, comprese le registrazioni e i post di blog, sarà condiviso con i partecipanti, fornendo una forma documentata del contenuto della sessione.
   * I partecipanti sono stati incoraggiati a contattare i propri TAM o CSM per ulteriore assistenza e a esplorare le licenze Ultimate Success per sessioni di coaching personalizzate.
