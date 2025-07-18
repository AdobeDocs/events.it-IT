---
title: 'AEM GEM: guida introduttiva ad Adobe Managed CDN'
description: Scopri come configurare Adobe Managed CDN in AEM Cloud Service per migliorare le prestazioni e la sicurezza con le nuove funzionalità di configurazione CDN.
role: Developer, User
level: Intermediate
feature: Edge Delivery Services
doc-type: Event
duration: 3438
last-substantial-update: 2025-01-30T00:00:00Z
jira: KT-17227
exl-id: 4cd0332f-95bf-45f4-a765-aba020c0d7b0
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# AEM GEM: guida introduttiva ad Adobe Managed CDN

Scopri la rete CDN gestita di Adobe in AEM Cloud Service e come configurarla. Unisciti a noi per esplorare le nuove funzionalità di configurazione CDN che possono essere utilizzate per migliorare sia le prestazioni che la sicurezza delle applicazioni AEM as a Cloud Service. In questa sessione scoprirai:

* Cos’è Adobe CDN
* Topologie rilevanti per AEMaaCS e Edge Delivery Services
* Casi d’uso tipici che possono essere implementati con le regole CDN
* Come utilizzare gli RDE per testare e distribuire rapidamente le configurazioni CDN

>[!VIDEO](https://video.tv.adobe.com/v/3443168/?learn=on&enablevpops)

*Registrato il 22 gennaio 2025*

Hai una domanda, forse un commento?  Partecipa alla discussione in [Experience League Communities](https://adobe.ly/4haufPK)!

## Punti chiave da eliminare

### Funzioni chiave di Adobe Managed CDN

* **Domini e certificati personalizzati** Essenziali per l&#39;hosting di domini e certificati personalizzati per stabilire connessioni sicure.
* **Memorizzazione in cache** La consegna di risposte HTTP dalla cache è molto più veloce (meno di 10 millisecondi) rispetto al recupero dall&#39;origine (centinaia di millisecondi).
* **CDN preconfigurata e personalizzata** Adobe fornisce una rete CDN gestita preconfigurata, ma gli utenti possono anche utilizzare una propria rete CDN.

### Opzioni di configurazione

* **Richiedi trasformazioni** Modifica intestazioni, percorsi di riscrittura, blocco del traffico e richieste di reindirizzamento.
* **Filtri di traffico** Blocca o consente il traffico in base a regole specifiche.
* **Autenticazione** Supporto per chiave perimetrale, chiave perforata e autenticazione di base.
* **Selettori origine** richieste proxy a origini diverse in base a regole definite.
* **Trasformazioni risposta** Modificare le intestazioni e lo stato delle risposte.

### Distribuzione e personalizzazione

* **Pipeline di configurazione** Distribuisci i file YAML per configurare le regole CDN.
* **Protezione traffico** Utilizza le regole del filtro del traffico per bloccare, registrare e avvisare il traffico in base ai modelli.
* **Limitazione frequenza** Proteggi da attacchi DDoS limitando il numero di richieste per IP.

### Strumenti e analisi

* **Stack Elasticsearch Kibana** Analizza l&#39;utilizzo e il traffico con le dashboard fornite.
* **Inoltro log** Inoltra i log a un&#39;istanza Splunk per l&#39;analisi.

### Elementi di rilievo demo

* **Distribuzione delle configurazioni** È stata dimostrata la distribuzione delle regole del filtro del traffico e dei reindirizzamenti.
* **Autenticazione e selezione origine** ha mostrato come impostare l&#39;autenticazione di base e il traffico proxy per origini diverse.

### Best practice

* **Risposte rapide** Assicurati risposte rapide dalle origini per evitare vulnerabilità.
* **Memorizzazione in cache corretta** Sfrutta la memorizzazione in cache per gestire il traffico in modo efficiente.
* **Usa dashboard** Analizza il traffico e l&#39;utilizzo per impostare i limiti di velocità appropriati.
* **Combina strategie** Utilizza strategie di limitazione della velocità diverse per una migliore protezione.
* **Imposta avvisi** Ricevi una notifica quando il sito è sotto attacco.
* **Verifica regole** Prima di bloccare, inizia con la registrazione delle azioni per garantire che le regole funzionino come previsto.

### Contatti e feedback

* **Feedback e casi d&#39;uso** Rivolgiti al team per ottenere feedback e casi d&#39;uso avanzati.
* **Sessioni future** Partecipa ai sondaggi per suggerire argomenti per le sessioni future.
