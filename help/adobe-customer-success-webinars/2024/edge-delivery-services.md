---
title: Ottimizzazione della distribuzione dei contenuti - Sfruttare la potenza dei servizi Edge
description: I Edge Delivery Services ATM (EDS) migliorano le funzionalità ATM con servizi componibili, cicli di sviluppo rapidi e punteggi di faro elevati, supporto di authoring basato su documenti e WYSIWYG, architettura senza server, creazione rapida di siti e opzioni di personalizzazione estese.
solution: Experience Manager, Experience Manager as a Cloud Service
feature: Edge Delivery Services
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3589
last-substantial-update: 2024-12-06T00:00:00Z
jira: KT-16631
source-git-commit: 47ae42d06ed311e60ebce194e0683bb95e8e5b69
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---


# Ottimizzazione della distribuzione dei contenuti: sbloccare la potenza dei servizi Edge

In questa sessione verrà fornita una panoramica dei Edge Delivery Services (EDS) e della relativa architettura. Verranno approfonditi i modi in cui EDS si integra con l’authoring basato su documenti e l’authoring basato su AEM tramite l’editor universale. Una demo live mostrerà l&#39;EDS in azione, seguita da risorse per ulteriori esplorazioni e una sessione Q&amp;A.

>[!VIDEO](https://video.tv.adobe.com/v/3440938/?learn=on&enablevpops)

## Punti chiave da eliminare

### Introduzione a EDS

* L&#39;EDS è un insieme di servizi componibili concepiti per migliorare le capacità dell&#39;ATM. &#x200B;
* Mira a fornire esperienze eccezionali che guidano coinvolgimento e conversioni con cicli di sviluppo rapidi e un punteggio del faro del 100%. &#x200B;

### Opzioni di authoring

* **Authoring basato su documenti** Utilizza strumenti familiari come Microsoft Word o Google Docs per la creazione di contenuti, consentendo la creazione rapida di contenuti senza formazione approfondita. &#x200B;
* **Universal Editor** Fornisce un&#39;interfaccia WYSIWYG simile ai siti ATM tradizionali, consentendo la creazione di contenuti più dettagliati e visivi. &#x200B;

### Architettura

* EDS si integra all’interno del framework di Cloud Service Amazon. &#x200B;
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
* Gli utenti sono invitati a contattare il supporto di Adobe per eventuali problemi non risolti. &#x200B;