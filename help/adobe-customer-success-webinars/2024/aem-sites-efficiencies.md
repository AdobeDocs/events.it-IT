---
title: 'Efficienza di AEM Sites: ottimizzazione delle prestazioni, configurazione e risoluzione dei problemi'
description: nozioni di base sulla risoluzione dei problemi dei siti Adobe Experience Manager (AEM). Che tu stia affrontando problemi di prestazioni o che stai gestendo configurazioni complesse, questa sessione fornirà competenze pratiche per mantenere e ottimizzare il tuo ambiente AEM. Daremo priorità alle demo live rispetto alle diapositive, offrendo un’esperienza pratica nell’affrontare le sfide del mondo reale​.Punti principali di discussione:- Configurazione host virtuale e mappatura dominio- Problemi di prestazioni- Autorizzazione, identificazione, autorizzazioni utente
solution: Experience Manager
version: Cloud Service
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3452
last-substantial-update: 2024-10-30T00:00:00Z
jira: KT-16353
source-git-commit: 3f245f71cd4db5097b5a9e712114112451d899e4
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---


# Efficienza di AEM Sites: ottimizzazione delle prestazioni, configurazione e risoluzione dei problemi

In questo webinar approfondiremo le nozioni di base sulla risoluzione dei problemi dei siti Adobe Experience Manager (AEM). Che tu stia affrontando problemi di prestazioni o che stai gestendo configurazioni complesse, questa sessione fornirà competenze pratiche per mantenere e ottimizzare il tuo ambiente AEM. Daremo priorità alle demo live rispetto alle diapositive, offrendo un’esperienza pratica nell’affrontare le sfide del mondo reale&#x200B;.

>[!VIDEO](https://video.tv.adobe.com/v/3435114/?learn=on)

## Punti chiave

Il webinar si è concentrato sull’efficienza del sito AMP, tra cui l’ottimizzazione delle prestazioni, la configurazione e la risoluzione dei problemi.

### Configurazione Dispatcher

* Importanza del dispatcher per la distribuzione di siti web performanti.
* Aspetti chiave della configurazione del dispatcher: configurazione dell’host virtuale, mappatura del dominio con struttura della cache e rapporti e reindirizzamenti regolari.

### Rights Management

* Best practice: applica i diritti ai gruppi, evita le istruzioni di negazione ed evita la sovra-progettazione.
* Utilizzo dello strumento ACL Netcentric per la gestione dei diritti tramite un file Yaml, garantendo facilità di distribuzione e tracciabilità.

### Problemi relativi alle prestazioni

* Importanza di identificare i delta nelle operazioni di sincronizzazione per evitare il flushing completo della cache.
* Evita operazioni di pagina di grandi dimensioni durante l’orario di lavoro.
* Semplificare i flussi di lavoro secondo i passaggi necessari.
* Presta attenzione ai processi di sistema di terze parti sui sistemi di authoring, in particolare con strumenti come ImageMagick.
* Evita richieste sincronizzate con sistemi di terze parti che non possono gestire il carico.
* Gestisci i componenti personalizzati pesanti per evitare il deterioramento delle prestazioni.
* Monitora le sessioni a lunga durata per evitare eccezioni di segmenti non trovati.