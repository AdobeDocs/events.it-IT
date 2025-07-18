---
title: Ambienti di sviluppo rapido Adobe Experience Manager
description: Semplifica lo sviluppo e l’implementazione rapidi in ambienti cloud con il nuovo SDK di Adobe, riducendo notevolmente i tempi di implementazione e supportando aggiornamenti rapidi, registri live e opzioni di configurazione avanzate, come descritto in DevOps Life 2024.
solution: Experience Manager as a Cloud Service, Experience Manager
feature: Developer Tools
topic: Development
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2427
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16570
exl-id: 330d8be1-14a0-488a-aae0-ee90e1f7621e
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Ambienti di sviluppo rapido Adobe Experience Manager

Esplora le best practice per gli ambienti di sviluppo rapido (RDE) e la console per sviluppatori aggiornata. Natalia Angulo Herrera, Software Development Engineer presso Adobe, e Remo Liechtenstein, Software Development Engineer presso Adobe, illustrano le problematiche relative alla migrazione, la configurazione della CLI dell&#39;AIO, l&#39;installazione, i test, la registrazione e la gestione della configurazione per un flusso di lavoro Adobe Experience Manager più fluido.

>[!VIDEO](https://video.tv.adobe.com/v/3440397/?learn=on&enablevpops)


## Discussione community

Continua la conversazione nella [discussione](https://adobe.ly/3UJluDo) della community Adobe Developers Live.

## Punti chiave da eliminare

* **Introduzione a DevOps Life 2024** La sessione è ospitata da Natalia e Remo di Adobe e si concentra sugli ambienti di sviluppo rapido.
* **Istruzione del problema** La sfida degli ambienti di sviluppo locali che funzionano correttamente localmente ma non riescono quando vengono distribuiti nel cloud.
* **Soluzione** Creazione di un nuovo SDK nel cloud per facilitare lo sviluppo e la distribuzione rapidi, riducendo il tempo da 30 minuti a secondi o alcuni minuti.
* **Processo di distribuzione** Il nuovo ambiente consente di eseguire aggiornamenti e convalide rapidi tramite un nuovo plug-in API e CLI, consentendo un feedback e una distribuzione più rapidi.
* **Differenze di infrastruttura** L&#39;ambiente cloud utilizza una singola istanza di authoring e pubblicazione senza elevata disponibilità e non utilizza MongoDB.
* **Installazione e utilizzo** Gli sviluppatori possono configurare un ambiente di sviluppo rapido tramite l&#39;interfaccia cloud, utilizzando npm e Adobe IO CLI per l&#39;installazione e la configurazione.
* **Comandi di base** I comandi chiave includono io amd: help, io login, io status, io install, io history, io delete e io reset.
* **Registrazione e debug** Il nuovo ambiente supporta i registri attivi e la modifica dei livelli di registro senza ridistribuzione, utilizzando comandi come iO am o d logs.
* **Argomenti avanzati** Supporto per pacchetti front-end e pipeline di configurazione, per una distribuzione e iterazione rapide.
* **Prossime funzionalità** prevede di introdurre funzionalità snapshot per reimpostare l&#39;ambiente in modo più semplice e per eseguire aggiornamenti automatici senza perdita di contenuto.
* **Domande e risposte e feedback** La sessione incoraggia i partecipanti ad unirsi al canale Discord per interagire in tempo reale e fornire feedback con il team di sviluppo.
