---
title: Configurazione di CDN e WAF in Adobe Experience Manager as a Cloud Service
description: Migliora le prestazioni e la sicurezza delle applicazioni Adobe Experience Manager as a Cloud Service con regole CDN personalizzabili, protezione WAF e pipeline di configurazione, secondo quanto condiviso dagli esperti Adobe.
solution: Experience Manager as a Cloud Service
feature: Security
topic: Performance, Security
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2211
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16574
exl-id: a9f38e79-c707-443d-8b2f-e534ce4dd43d
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Configurazione di CDN e WAF in Adobe Experience Manager as a Cloud Service

Sfrutta appieno il potenziale della rete CDN gestita di Adobe con regole CDN personalizzabili, protezione WAF e pipeline di configurazione. Marius Petria, Sr. Computer Scientist di Adobe, Quentin Vecchio, Software Development Engineer di Adobe e Florian Froese, Software Development Engineer di Adobe, condividono strategie per migliorare le prestazioni e la sicurezza delle applicazioni Adobe Experience Manager as a Cloud Service.

>[!VIDEO](https://video.tv.adobe.com/v/3440401/?learn=on&enablevpops)

## Discussione community

Continua la conversazione nella [discussione](https://adobe.ly/3O0TyYa) della community Adobe Developers Live.

## Punti chiave

* **Introduzione di nuove funzionalità di configurazione** La presentazione introduce nuove funzionalità di configurazione per la rete CDN in un servizio cloud, concentrandosi sulla possibilità di configurare la rete CDN per vari casi d&#39;uso.
* **Opzioni di configurazione CDN** Le nuove opzioni consentono l&#39;interazione con le richieste e le risposte HTTP, ad esempio l&#39;aggiunta o la rimozione di intestazioni, la riscrittura dei percorsi delle richieste, il blocco del traffico, il reindirizzamento dei client e il proxy a origini diverse.
* **Miglioramenti della sicurezza** Le nuove funzionalità includono le regole del filtro del traffico per bloccare o registrare il traffico in base ai modelli di richiesta e l&#39;introduzione di M WAF per la protezione avanzata contro attacchi Web come SQL injection e XSS.
* **Configurazione dichiarativa** La configurazione viene eseguita utilizzando file YAML e distribuita tramite una pipeline di configurazione in Cloud Manager, rendendola un processo rapido e semplice.
* **Trasformazioni di richieste e risposte** Le nuove funzionalità consentono di normalizzare gli URL mediante trasformazioni di richieste e rimuovere parametri di query non necessari, nonché trasformazioni di risposta per impostare le intestazioni prima di inviare risposte ai client.
* **Filtri di traffico e limitazione della velocità** I filtri di traffico possono bloccare IP o paesi specifici e implementare la limitazione della velocità per proteggere dagli attacchi DDoS. La limitazione della frequenza può essere configurata in base a vari criteri come l’IP del client, l’agente utente e il percorso della richiesta.
* **Strumenti di monitoraggio e analisi** Adobe fornisce strumenti come Elasticsearch/Kibana e Splunk dashboard per analizzare il traffico e l&#39;utilizzo, aiutando a identificare e mitigare potenziali minacce per la sicurezza.
* **Demo pratica** La presentazione include una demo che mostra come distribuire le configurazioni CDN utilizzando Cloud Manager e come gestire gli errori e convalidare le configurazioni localmente utilizzando AEM.
