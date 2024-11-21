---
title: 'Efficienza di AEM Sites: ottimizzazione delle prestazioni, configurazione e risoluzione dei problemi'
description: Questa sessione descrive le competenze essenziali per la risoluzione dei problemi dei siti Adobe Experience Manager (AEM), incentrata su soluzioni pratiche per problemi di prestazioni, configurazioni complesse e autorizzazioni utente.
solution: Experience Manager
version: Cloud Service
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3452
last-substantial-update: 2024-10-30T00:00:00Z
jira: KT-16353
exl-id: 55f7c1d8-7c2c-4392-894a-2aa9b3cc0e4a
source-git-commit: ef652eb09c33f11d69ec66f70013cd3e53537a95
workflow-type: tm+mt
source-wordcount: '235'
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
