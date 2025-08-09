---
title: Best practice e informazioni approfondite per la modellazione di schemi XDM
description: La modellazione dei dati master in AEP con schemi XDM, gestione delle identità e best practice per la personalizzazione e la segmentazione scalabili e in tempo reale.
solution: Experience Platform
topic: Personalization
role: Developer
level: Intermediate
doc-type: Event
duration: 3488
last-substantial-update: 2025-05-08T00:00:00Z
jira: KT-18019
exl-id: 3327dc51-b5e4-49bd-884a-4defea8664eb
source-git-commit: ef1eacd73c5a4fb9cdfee730d40606ec65bab2a7
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Best practice e informazioni approfondite per la modellazione di schemi XDM

In questa sessione, scopri le best practice e le scelte rapide essenziali per la creazione di modelli XDM (Adobe Experience Data Model) scalabili e di alta qualità in linea con gli standard Adobe Experience Platform. Ottieni informazioni approfondite su come mappare in modo efficace i dati sull’esperienza del cliente e sui casi d’uso in XDM per un’integrazione fluida in Adobe e strumenti esterni.

## Punti di discussione

* Come definire e organizzare i componenti XDM per garantire modelli di dati scalabili e flessibili
* Sfide comuni nella progettazione, nell’evoluzione e nella manutenzione di XDM

>[!VIDEO](https://video.tv.adobe.com/v/3458042/?learn=on&enablevpops)

## Punti chiave da eliminare

**Modellazione dati in Adobe Experience Platform (AEP)**

Lo schema XDM è la base per la modellazione dei dati in AEP, consentendo l’integrazione e la condivisione dei dati tra sistemi diversi. Definisce la struttura e il significato dei dati, ad esempio gli attributi del profilo e le azioni basate su eventi.

**Identity Management**

Una corretta gestione delle identità è fondamentale per evitare problemi come il collasso del profilo. L’hashing di dati sensibili come le e-mail e l’utilizzo di identificatori univoci può contribuire a mantenere l’integrità dei dati. Le mappe di identità sono consigliate per la segmentazione e la personalizzazione in tempo reale.

**Best practice per la progettazione dello schema**

Mantieni gli schemi semplici e concentrati sui casi di utilizzo di marketing. Evita di sovraccaricare gli schemi con attributi non necessari. Utilizza gruppi di campi standardizzati e riduci al minimo le personalizzazioni per garantire scalabilità e affidabilità nel futuro.

**Evento - Attributi del profilo**

Decidi se modellare i dati come attributi di profilo o eventi in base agli obiettivi di marketing. Gli attributi del profilo sono adatti al targeting in tempo reale, mentre gli eventi forniscono informazioni storiche sulla segmentazione basata sul tempo.

**Gestione di profili compressi e scalabilità**

I profili compressi possono essere corretti solo dal supporto di Adobe, ma le regole del grafo delle identità possono evitare collassi futuri. Per ristrutturare gli schemi esistenti, si consiglia di estrarre i dati necessari e iniziare da zero con uno schema pulito.
