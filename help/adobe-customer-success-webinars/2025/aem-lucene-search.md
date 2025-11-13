---
title: Suggerimenti e best practice essenziali per AEM Lucene Search
description: Aumenta il coinvolgimento digitale con strumenti di ricerca avanzati di AEM come filtri, facet, suggerimenti automatici, NGram e controllo ortografico. Impara dalle demo del mondo reale.
solution: Experience Manager
feature: Search
role: Admin, Developer
level: Intermediate, Experienced
doc-type: Event
duration: 3630
last-substantial-update: 2025-11-13T00:00:00Z
jira: KT-19550
source-git-commit: 84c9a126769fa94b0197d12ca594137e13edc510
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---


# Suggerimenti e best practice essenziali per AEM Lucene Search

Scopri come migliorare la tua presenza digitale e il coinvolgimento dei clienti con funzioni di ricerca all’avanguardia, tra cui filtri, facet, suggerimenti automatici, NGram e controllo ortografico. Scopri le funzionalità di AEM e Lucene e acquisisci informazioni su come ottimizzarle. Questo webinar offre l’opportunità di migliorare la tua esperienza di ricerca e rimanere all’avanguardia nel panorama digitale.

>[!VIDEO](https://video.tv.adobe.com/v/3476410/?learn=on&enablevpops)

## Sblocco di ricerche avanzate in Adobe Experience Manager

Adobe Experience Manager (AEM) sfrutta la funzione di ricerca di Lucene per fornire risultati rapidi e pertinenti per contenuti, risorse e metadati. Questa sessione esplora il funzionamento degli indici Lucene, come configurarli e le best practice per massimizzare le prestazioni di ricerca.

* **La ricerca Lucene è ovunque** Consente di eseguire ricerche in AEM Author, Publisher e Portals, nonché di gestire suggerimenti automatici, filtri, facet e impaginazione.
* **Prestazioni unità delle definizioni degli indici** La personalizzazione delle definizioni degli indici Oak è fondamentale per una ricerca efficiente e mirata.
* **Argomento sulle best practice** Copia le definizioni degli indici esistenti, limita le proprietà indicizzate e utilizza i flag giusti per le ricerche full-text e delle proprietà.
* **Funzionalità avanzate per migliorare l&#39;esperienza utente** È possibile abilitare facet, suggerimenti automatici, controllo ortografico, potenziamento e stemming per esperienze di ricerca più ricche.

Comprendere questi principi aiuta a garantire funzionalità di ricerca stabili e di alto valore in AEM, supportando sia gli obiettivi tecnici che quelli aziendali.

## Blocchi predefiniti dell’indice Lucene

Le definizioni dell’indice AEM Lucene sono alla base delle prestazioni e della precisione della ricerca. I componenti chiave includono:

* **Tipo** Specifica il tipo di indice (Lucene, proprietà, ecc.).
* **Restrizione del tipo di nodo** ha come destinazione tipi di contenuto specifici (ad esempio, dam:Asset, cq:Page).
* **Limitazione percorso** limita l&#39;indicizzazione ai percorsi dell&#39;archivio definiti per migliorarne l&#39;efficienza.
* **Regole di aggregazione** Controlla la profondità e l&#39;ambito del contenuto indicizzato, assicurando che le proprietà rilevanti siano ricercabili.
* **Regole indice** Configurazione di base; imposta flag come nodeScopeIndex (ricerca full-text ampia) e analizzati (tokenizzazione/normalizzazione).

L’attenta configurazione di questi elementi garantisce che le query di ricerca siano veloci, pertinenti ed efficienti dal punto di vista delle risorse.

## Ottimizzazione delle prestazioni di ricerca

Un’efficace ottimizzazione della ricerca in AEM Lucene comporta una configurazione strategica e il rispetto delle best practice:

* **Inizia con gli indici esistenti** Copia e modifica sempre le definizioni pronte all&#39;uso, senza generare da zero.
* **Limita proprietà indicizzate** Includi solo le proprietà necessarie per mantenere gli indici snelli e performanti.
* **Utilizzare I Flag In Modo Saggio:
   * **nodeScopeIndex** true per ricerche full-text estese
   * **analizzato** true per la tokenizzazione a livello di proprietà
   * **evaluatePathRestriction** true per le query basate su percorsi
* **Indicizzazione proprietà** Per ottenere prestazioni ottimali, preferisci le ricerche con restrizioni delle proprietà. Utilizza solo testo completo quando necessario.
* **Ordinamento e facet** Abilita propertyIndex e ordina l&#39;ordinamento; imposta facet** true per il filtro basato sul conteggio.

L’applicazione di queste strategie consente di velocizzare le query, ridurre l’utilizzo delle risorse e ottenere risultati più rilevanti.

