---
title: Ottimizzazione della distribuzione dei contenuti - Sfruttare la potenza dei servizi Edge
description: La sessione su Edge Delivery Services (EDS) ha trattato l’architettura, l’integrazione con l’authoring basato su documenti e su AEM, la creazione rapida di siti, le opzioni di personalizzazione e le best practice per mantenere prestazioni elevate.
solution: Experience Manager, Experience Manager as a Cloud Service
feature: Edge Delivery Services
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3589
last-substantial-update: 2024-12-06T00:00:00Z
jira: KT-16631
exl-id: 2057e491-9ec3-4bfe-b85a-6b74d70822bf
source-git-commit: 32060a6a0d2cc24b8dc09c8f5e9f9d9c679e6d3e
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Ottimizzazione della distribuzione dei contenuti: sbloccare la potenza dei servizi Edge

In questa sessione verrà fornita una panoramica di Edge Delivery Services (EDS) e della relativa architettura. Verranno approfonditi i modi in cui EDS si integra con l’authoring basato su documenti e l’authoring basato su AEM tramite l’editor universale. Una demo live mostrerà l&#39;EDS in azione, seguita da risorse per ulteriori esplorazioni e una sessione Q&amp;A.

>[!VIDEO](https://video.tv.adobe.com/v/3440938/?learn=on&enablevpops)

## Punti chiave da eliminare

### Introduzione a EDS

* EDS è un insieme di servizi componibili progettati per migliorare le funzionalità di ATM. &#x200B;
* Mira a fornire esperienze eccezionali che guidano coinvolgimento e conversioni con cicli di sviluppo rapidi e un punteggio del faro del 100%. &#x200B;

### Opzioni di authoring

* **Authoring basato su documenti** Utilizza strumenti familiari come Microsoft Word o Google Docs per la creazione di contenuti, consentendo una creazione rapida dei contenuti senza formazione approfondita. &#x200B;
* **Universal Editor** Fornisce un&#39;interfaccia WYSIWYG simile ai siti ATM tradizionali, consentendo la creazione di contenuti più dettagliati e visivi. &#x200B;

### Architettura

* EDS si integra all’interno del framework Amazon Cloud Service. &#x200B;
* Supporta l’implementazione senza server e può funzionare senza un’istanza Autore o Autore tradizionale. &#x200B;
* È possibile implementare due livelli di caching: a livello di infrastruttura del cliente e a livello di EDS. &#x200B;

### Gestione dei contenuti

* L’authoring basato su documenti richiede un account GitHub, Google Drive o Microsoft SharePoint, un plug-in per la barra laterale e uno strumento di sincronizzazione del codice. &#x200B;
* EDS con authoring IAM richiede un account GitHub, una licenza IAM as a Cloud Service e uno strumento di sincronizzazione del codice.

### Sviluppo e implementazione

* Il processo di creazione di un sito con EDS è rapido e richiede spesso meno di un giorno. &#x200B;
* Lo sviluppo locale può essere eseguito utilizzando il comando aem up per creare una versione locale del sito web.
* È possibile eseguire il commit delle modifiche nei rami di funzionalità per il test prima di unirle al ramo principale. &#x200B;

### Personalizzazione ed estensibilità

* I componenti personalizzati possono essere creati utilizzando semplici CSS e JavaScript. &#x200B;
* L’architettura consente integrazioni di terze parti e origini di authoring personalizzate.

### Best practice

* Si consiglia di utilizzare Vanilla JavaScript e CSS per mantenere punteggi elevati nel faro.
* Qualsiasi introduzione di librerie come React deve essere attentamente considerata e testata per evitare il degrado delle prestazioni.

### Supporto e documentazione

* È disponibile una documentazione completa per guidare gli utenti durante il processo di configurazione e personalizzazione. &#x200B;
* Gli utenti sono invitati a contattare il supporto Adobe per eventuali problemi non risolti. &#x200B;
