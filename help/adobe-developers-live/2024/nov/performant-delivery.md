---
title: Best practice per la distribuzione performante
description: Ottimizza la distribuzione e le prestazioni dei contenuti multimediali con Dynamic Media sfruttando lo streaming adattivo, i profili video personalizzati, le best practice SEO, l’ottimizzazione delle immagini, la gestione di contenuti in blocco, i predefiniti per visualizzatori, l’invalidamento della cache e l’imaging intelligente.
feature: Dynamic Media, Video, SEO Optimization, Smart Imaging, Viewer Presets, Best Practices
topic: Content Management
solution: Experience Manager, Experience Manager Assets
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1596
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16572
exl-id: a1920020-b9ce-43be-8f9e-e52aac68da7b
source-git-commit: 946d7cd484e8c5d4358d4099b3518705cab8d4a3
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Best practice per la distribuzione performante

Unisciti a Riya Midha, Sr. Product Manager di Adobe, per scoprire le best practice per la configurazione di Adobe Experience Manager Assets Dynamic Media. Scopri come ottimizzare la distribuzione delle risorse, migliorare lo streaming video, configurare i visualizzatori e misurare e migliorare le prestazioni.

>[!VIDEO](https://video.tv.adobe.com/v/3440399/?learn=on&enablevpops)

## Discussione community

Continua la conversazione nella [discussione](https://adobe.ly/3YGedpb) della community Adobe Developers Live.

## Punti chiave da eliminare

* **Funzionalità Dynamic Media** Dynamic Media consente la distribuzione rapida e flessibile di contenuti multimediali personalizzati di alta qualità su dispositivi diversi, gestendo oltre 9.000 miliardi di consegne di contenuti multimediali all&#39;anno e picchi giornalieri di risorse fino a 69 miliardi.
* **Streaming adattivo** L&#39;utilizzo dello streaming adattivo per la distribuzione di video riduce in modo significativo il buffering. Un test ha mostrato una riduzione del numero di buffer da 50 a 5 su un video di 60 secondi con una larghezza di banda limitata di 5 Mbps.
* **Profili video** La creazione di profili video personalizzati con codifica di qualità diversa garantisce prestazioni video ottimali in condizioni di rete diverse.
* **Best practice per l&#39;ottimizzazione SEO**
   * Utilizza i set di regole per creare URL descrittivi per una SEO migliore.
   * Aggiungete testo alternativo e attributi del titolo alle immagini.
   * Utilizza l’imaging avanzato e i formati di immagine più recenti, come WebP, per una migliore classificazione delle ricerche.
* **Ottimizzazione immagine**
   * Usate i parametri di scala per regolare la risoluzione dell&#39;immagine in base alle dimensioni dello schermo.
   * Evita di usare una qualità del 100% per le immagini; utilizza invece un intervallo di 80-90% per ridurre le dimensioni del file senza perdite di qualità evidenti.
   * Applica parametri di nitidezza per migliorare la chiarezza del testo nelle immagini.
* **Gestione contenuto in blocco**
   * Separa i contenuti destinati alla distribuzione di contenuti Dynamic Media da altri contenuti.
   * Utilizza la sincronizzazione selettiva per ottimizzare i tempi di elaborazione e migliorare i tempi di commercializzazione.
* **Predefiniti visualizzatore** Personalizza l&#39;aspetto e il comportamento del visualizzatore utilizzando i predefiniti visualizzatore senza modifiche al codice. Alcuni esempi includono la modifica dei pulsanti di riproduzione/pausa, l’abilitazione della riproduzione automatica e del ciclo continuo e l’aggiunta di sovrapposizioni di immagini.
* **Annullamento della validità della cache** Utilizza l&#39;annullamento della validità della cache per riflettere immediatamente le modifiche apportate alle risorse già pubblicate, ignorando il valore TTL predefinito di 10 ore.
* **Monitoraggio e debug** Utilizza strumenti come l&#39;app desktop AEM e la pagina Query debugger per tenere traccia dei processi di elaborazione e identificare le risorse non elaborate.
* **Smart imaging** Per impostazione predefinita, Smart imaging è abilitato in tutti i domini, riducendo le dimensioni dei file di immagine e migliorando i tempi di caricamento.
