---
title: Padroneggiare gli elementi multimediali dinamici con Open API
description: Scopri le differenze principali tra gli elementi multimediali tradizionali e il modello Open API, e come eseguire correttamente la transizione e implementare Dynamic Media Ultimate con Open API.
solution: Experience Manager as a Cloud Service, Experience Manager Assets
feature-set: Experience Manager Assets
feature: SDK/API
topic: Development, Content Management
role: Admin, Developer, User
level: Beginner, Intermediate
doc-type: Event
duration: 2757
last-substantial-update: 2025-08-08T00:00:00Z
jira: KT-18702
source-git-commit: ef1eacd73c5a4fb9cdfee730d40606ec65bab2a7
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---


# Padroneggiare gli elementi multimediali dinamici con Open API

Questo webinar è progettato per professionisti che hanno familiarità con gli elementi multimediali dinamici tradizionali e desiderano comprendere e implementare [Dynamic Media Ultimate](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dm-prime-ultimate) con API aperte.  Esploreremo il funzionamento ad alto livello di Dynamic Media Ultimate con Open API e lo confronteremo con la versione tradizionale di Dynamic Media. Il nostro obiettivo è quello di fornire una comprensione completa delle differenze tra questi due approcci, consentendo ai partecipanti che hanno familiarità con Dynamic Media di adattarsi facilmente al modello Open API.

>[!VIDEO](https://video.tv.adobe.com/v/3470620/?learn=on&enablevpops)

## Caratteristiche principali a confronto

| Funzione | Contenuti multimediali dinamici | Dynamic Media con OpenAPI |
|-----------------------------|------------------------|----------------------------|
| *Disponibilità* | On-premise, AMS, Cloud | Solo cloud |
| *Modificatori* | Set completo disponibile | Limitato ma in crescita |
| *Controllo dell’accesso* | Apri a tutti gli utenti | Limitato da ruoli |
| *TTL CDN* | ~10 ore | ~10 minuti |
| *Imposizione approvazione* | Pubblicazione automatica | Richiede l&#39;approvazione |
| *SEO-friendly* | Sì | Sì |

## Scenari di integrazione

Questi scenari di integrazione dimostrano la flessibilità e la scalabilità di Dynamic Media con OpenAPI per diverse esigenze aziendali.

* **Integrazione AEM Sites** Dynamic Media con OpenAPI supporta l&#39;integrazione diretta con AEM Sites, consentendo il recupero delle risorse direttamente dal livello di consegna senza duplicazioni.
* **CMS** di terze parti consente l&#39;integrazione con piattaforme come Salesforce e Drupal tramite API o microapplicazioni front-end.
* **Accesso basato su API** fornisce API per la ricerca, il recupero e la distribuzione di rappresentazioni ottimizzate delle risorse.
* **Ottimizzazione del livello di consegna** Assets viene fornito tramite Fastly, garantendo una consegna più rapida ed efficiente.