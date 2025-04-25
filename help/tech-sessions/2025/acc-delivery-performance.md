---
title: Prestazioni consegna Adobe Campaign Classic - Risoluzione dei problemi
description: Questa sessione ha trattato strategie chiave per migliorare le prestazioni di consegna di e-mail e SMS tramite Adobe Campaign. Ha affrontato problematiche comuni quali ritardi di consegna, bassa velocità effettiva e lentezza delle transazioni, offrendo soluzioni quali l'ottimizzazione in batch, la registrazione SQL e il monitoraggio delle prestazioni dei server. Le best practice per la consegna dei messaggi includevano l’autenticazione e-mail corretta (SPF, DKIM, DMARC), il monitoraggio della blacklist e i controlli di posta indesiderata. Per migliorare le prestazioni, gli esperti hanno consigliato di pulire i flussi di lavoro, limitare le regole ed evitare contenitori condivisi. Suggerimenti per la consegna di SMS incentrati sulla corretta configurazione dell’account esterno e sull’analisi del registro. La sessione ha anche sottolineato la convalida del tracciamento, la manutenzione del database utilizzando rapporti gonfiati e l'applicazione di regole di pressione/affaticamento per aumentare il coinvolgimento. Una registrazione della sessione verrà condivisa tramite e-mail e pubblicata sul sito Adobe Experience.
version: Classic v7
solution: Campaign Classic v7
product: Adobe Campaign
feature: SMS, Deliverability, Troubleshooting
role: User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 2257
last-substantial-update: 2025-04-25T00:00:00Z
jira: KT-17869
source-git-commit: 373605f79b3122382e221252232a26535ff3109b
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---


# Sessioni tecniche: prestazioni di consegna Adobe Campaign Classic - Risoluzione dei problemi

In questa sessione verranno analizzate le problematiche comuni che si verificano durante la fornitura di prestazioni ottimali con Adobe Campaign Classic (ACC) e verranno fornite strategie utilizzabili per la risoluzione e la risoluzione dei problemi. I partecipanti impareranno a identificare i colli di bottiglia delle prestazioni, ad affrontare le incoerenze nella preparazione/configurazione della consegna e ad implementare le best practice per garantire comunicazioni fluide. Dall’ottimizzazione delle consegne al superamento delle difficoltà tecniche, questo webinar offrirà ai partecipanti le conoscenze e gli strumenti necessari per migliorare l’efficienza delle campagne ACC, ottenere risultati migliori e fornire esperienze cliente di alta qualità.

>[!VIDEO](https://video.tv.adobe.com/v/3457826/?learn=on&enablevpops)

## Punti chiave da eliminare

**Soluzioni e problemi di consegna**

* I problemi più comuni includono ritardi di consegna, errori di preparazione, consegne bloccate, tassi di successo bassi, throughput basso, coinvolgimento ridotto e lentezza di consegna transazionale.
* Le soluzioni includono l’ottimizzazione della gestione in batch delle consegne, il monitoraggio delle prestazioni del server, l’abilitazione della registrazione delle query SQL, la revisione dei registri di audit e la garanzia di una corretta configurazione delle affinità MTA e IP.

**Best practice per la consegna**

* Assicurati la corretta autenticazione delle e-mail (SPF, DKIM, DMARC).
* Monitora gli stati della blacklist ed evita contenuti che attivino la posta indesiderata.
* Utilizza i controlli anti-spam per valutare i punteggi anti-spam prima di inviare e-mail.

**Ottimizzazione delle prestazioni di consegna**

* Utilizza flussi di lavoro di targeting puliti e limita i campi di personalizzazione.
* Implementa regole di limitazione, elaborazione batch e regole di topologia per esclusioni e filtri.
* Evita di condividere i contenitori su più canali per evitare colli di bottiglia.

**Risoluzione dei problemi di consegna SMS**

* Assicurati che gli account esterni siano configurati in modo univoco e che i processi SMS siano in esecuzione.
* Controlla i registri SMS per individuare eventuali errori e verifica le espressioni regolari nelle impostazioni SMP.
* Rivolgersi al provider di servizi per problemi di configurazione errata.

**Lentezza della consegna transazionale**

* Monitora i tempi di elaborazione interni e totali.
* Assicurati che la dimensione di consegna rientri nei limiti (60 GB per batch, 30 GB per evento).
* Rivedi le regole di tipologia e le impostazioni di personalizzazione.

**Tracciamento e coinvolgimento**

* Convalida i flussi di lavoro di tracciamento e i registri del server.
* Prima della produzione, verifica le formule di tracciamento personalizzate in ambienti inferiori.
* Verificare che i server di tracciamento siano funzionanti.

**Manutenzione del database**

* Utilizza i rapporti di gonfiore per identificare le tabelle con un gonfiore elevato e giustificare un vuoto di database.

**Consigli generali**

* Utilizza le regole di pressione e di affaticamento per limitare le e-mail non necessarie.
* Segmenta le consegne di grandi dimensioni in batch più piccoli per ottimizzare le prestazioni.