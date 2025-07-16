---
title: Best practice per la migrazione ad Adobe Customer Journey Analytics da Adobe Analytics
description: Scopri i passaggi essenziali e le best practice per la migrazione da Adobe Analytics a Customer Journey Analytics (CJA), tra cui la progettazione dello schema XDM, la mappatura dei dati e la configurazione della visualizzazione dati.
solution: Analytics, Customer Journey Analytics
topic: Migration
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 3654
last-substantial-update: 2025-07-16T00:00:00Z
jira: KT-18535
source-git-commit: 90eb4a9d2cf445c58fde776092fb047f820fa207
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Best practice per la migrazione ad Adobe Customer Journey Analytics da Adobe Analytics

Scopri la migrazione da Adobe Analytics a Customer Journey Analytics (CJA). Ospitata da Nicolina Picone e Maurizio Corò del team Ultimate Success di Adobe, la sessione offre una panoramica approfondita di CJA, delle sue funzionalità e delle best practice per la migrazione.

## Argomenti principali trattati

* differenze tra Analytics e CJA
* l’importanza di identificatori di identità affidabili, dell’allineamento delle strutture di dati e della creazione di visualizzazioni dati personalizzabili
* illustra le strategie per importare dati storici, gestire l’attribuzione del canale di marketing e sfruttare la flessibilità di CJA per la generazione di rapporti personalizzati

>[!VIDEO](https://video.tv.adobe.com/v/3464911/?learn=on&enablevpops)

## Principali percorsi

* **Panoramica di Customer Journey Analytics (CJA)** CJA è un&#39;evoluzione di Adobe Analytics e si concentra sull&#39;intero percorso di clienti in più punti di contatto (ad esempio, dispositivi mobili, web, CRM, call center) anziché in eventi a traccia singola. Consente l’elaborazione e la manipolazione dei dati in tempo reale.

* **Preparazione alla migrazione** I passaggi chiave per la migrazione da Adobe Analytics a CJA includono la verifica di un identificatore di identità sicuro (ad esempio, ID persona), l&#39;allineamento di variabili e dimensioni e la mappatura dei dati sullo schema XDM. I dati storici possono essere importati con passaggi di convalida.

* **Visualizzazioni dati e flessibilità** CJA consente la creazione di visualizzazioni dati personalizzabili con durate di sessione, filtri di segmentazione e impostazioni di attribuzione regolabili. Questa flessibilità consente reporting e analisi personalizzati.

* **Procedure consigliate per la migrazione cronologica dei dati** Convalida i dati di CJA confrontandoli con i dati di Adobe Analytics entro un intervallo accettabile (ad esempio, differenza del 10%). Inizia con una breve finestra di backfill (ad esempio, un mese) e aumenta gradualmente.

* **Marketing Channel Attribution** CJA offre funzionalità avanzate per l&#39;attribuzione dei canali di marketing, eliminando limitazioni quali la funzione &quot;prima pagina di visita&quot; e abilitando configurazioni di sessione più dinamiche.
