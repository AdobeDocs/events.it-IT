---
title: 'Ottimizzazione delle prestazioni di AEM: strategie e tecniche di caching'
description: La sessione ha trattato strategie e tecniche di caching, meccanismi e livelli di caching, gestione dinamica dei contenuti, problemi di debug della cache e sincronizzazione dell’invalidamento della cache tra Dispatcher e CDN.
topic: Performance
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3764
last-substantial-update: 2025-02-21T00:00:00Z
jira: KT-17373
source-git-commit: e7bf8b79ad4920b303fc3afbdfb4adee60614c88
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---


# Ottimizzazione delle prestazioni di AEM: strategie e tecniche di caching

In questa sessione esploriamo vari meccanismi di caching, come la memorizzazione in cache di pagine, risorse e dispatcher, nonché come implementare il caching a livello CDN per ottimizzare la distribuzione dei contenuti e ridurre i tempi di caricamento. La discussione tratterà le best practice per ogni livello di caching, la risoluzione dei problemi comuni e come sfruttare le funzionalità CDN per massimizzare l’efficienza.

## Punti principali di discussione

* Introduzione al caching
* Tipi di caching, best practice per la memorizzazione in cache, annullamento della validità e aggiornamento della cache
* Tecniche di debug

>[!VIDEO](https://video.tv.adobe.com/v/3444452/?learn=on&enablevpops)

## Punti chiave da eliminare

* **Strategie e tecniche di caching** La sessione si è concentrata su varie strategie e tecniche di caching per ottimizzare le prestazioni, incluso il caching a diversi livelli come browser, CDN e dispatcher.

* **Meccanismi di memorizzazione in cache e livelli** La discussione ha riguardato diversi meccanismi e livelli di memorizzazione in cache, tra cui memorizzazione in cache del browser, memorizzazione in cache CDN e memorizzazione in cache del dispatcher, e come configurarli e gestirli.

* **Gestione dinamica dei contenuti** Sono state discusse le tecniche per la gestione dei contenuti dinamici su una pagina, incluso l&#39;utilizzo di Sling Dynamic Include (SDI) e Edge Side Includes (ESI) per garantire che il contenuto dinamico non venga memorizzato nella cache mentre il contenuto statico lo è.

* **Problemi di debug della cache** Sono state illustrate diverse tecniche per eseguire il debug dei problemi di caching a diversi livelli (browser, CDN, dispatcher), incluso l&#39;utilizzo di intestazioni, registri e configurazioni specifiche per identificare e risolvere i problemi di caching.

* **Sincronizzazione dell&#39;invalidazione della cache** La sessione ha risolto il problema della sincronizzazione dell&#39;invalidazione della cache tra Dispatcher e CDN, consigliando l&#39;uso di valori di età massima più brevi e di API di eliminazione CDN per garantire che entrambe le cache vengano invalidate contemporaneamente all&#39;attivazione della pagina.