---
title: Architettura di Analysis - Come avvicinarsi al modello dati di Customer Journey Analytics
description: Scopri come strutturare i modelli dati di CJA con gerarchie di eventi, attribuzione e KPI per acquisire informazioni più approfondite sul percorso dei clienti.
feature: Attribution
topic: Administration
role: User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 0
last-substantial-update: 2025-09-04T00:00:00Z
jira: KT-18813
exl-id: 704ff998-840a-4815-a24f-f08b625b14f5
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Architettura dell’analisi: come approcciare il modello dati di Customer Journey Analytics

Un aspetto fondamentale della creazione di un modello dati di CJA è la comprensione della relazione gerarchica tra diversi punti di contatto e interazioni. Questo costituisce la base per analisi e approfondimenti significativi.

Le considerazioni principali includono:

* Identificazione e mappatura dei punti di interazione del cliente su tutti i canali
* Definizione di chiare gerarchie e relazioni di eventi
* Definizione di modelli di attribuzione coerenti
* Creazione di metriche e KPI standardizzati

Strutturando correttamente questi elementi, le organizzazioni possono monitorare e analizzare meglio l’intero percorso dei clienti, fornendo informazioni più fruibili e migliorando le capacità decisionali.

>[!VIDEO](https://video.tv.adobe.com/v/3471111/?learn=on&enablevpops)

## Sblocco della modellazione dati per analisi potenti

Scopri come l’architettura dei dati in Adobe Experience Platform (AEP) e Customer Journey Analytics (CJA) offre informazioni e rapporti utili.

* **Aspetti relativi alla progettazione dello schema** La scelta tra schemi piatti, array e array di oggetti influisce direttamente sulle funzionalità di analisi e sulla flessibilità di reporting.
* **Processo di trasformazione** I dati acquisiti in AEP devono essere strutturati accuratamente per garantire una trasformazione e un utilizzo senza soluzione di continuità in CJA.
* **Gerarchia dei contenitori** La comprensione dei livelli di evento, sessione e persona è fondamentale per l&#39;analisi a più livelli e la creazione di rapporti accurati.
* **Strategie pratiche** La pianificazione anticipata, la governance dello schema e l&#39;utilizzo delle funzionalità della piattaforma sono fondamentali per implementazioni scalabili e a prova di futuro.

La padronanza di questi concetti consente ai team di ottimizzare i flussi di lavoro di analisi e ottenere informazioni aziendali più approfondite.

## Tipi di schema e relativi casi d’uso

* **Schemi piatti** Ideale per relazioni di dati uno a uno semplici. Ideale per il tracciamento degli eventi di base e metriche/dimensioni semplici.
* **Array** Utili per elenchi di elementi correlati (ad esempio, categorie di prodotti, tag di contenuto). Ogni elemento array diventa una dimensione individuale per l&#39;analisi.
* **Array di oggetti** progettati per casi d&#39;uso complessi, ad esempio acquisti di prodotti, in cui ogni oggetto mantiene le proprie proprietà e relazioni. Consente un&#39;analisi dettagliata a livello di oggetto.
* **Scelta saggia** Seleziona lo schema più semplice che soddisfi le tue esigenze, ma sfrutta array e oggetti per scenari avanzati che richiedono la conservazione delle relazioni.
