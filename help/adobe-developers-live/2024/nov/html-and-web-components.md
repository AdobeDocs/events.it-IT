---
title: Eseguire il roll-out del proprio HTML con i componenti Web
description: Scopri le nozioni di base di Web Components con Raymond Camden, Sr. Developer Evangelist di Adobe, inclusi elementi personalizzati, DOM shadow e modelli HTML, con esempi pratici come l’incorporamento di PDF e la creazione di tabelle ordinabili per migliorare le applicazioni.
topic: Development
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2580
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16579
source-git-commit: 8770c8172ee90524079efc65aec7e129f1d1d031
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---


# Eseguire il roll-out del proprio HTML con i componenti Web

Raymond Camden, Sr. Developer Evangelist di Adobe, spiega le nozioni di base su Web Components, inclusi gli elementi personalizzati, Shadow DOM e i modelli di HTML. Esplora esempi reali come l’incorporamento di PDF e la creazione di tabelle ordinabili per migliorare le applicazioni con soluzioni moderne e riutilizzabili.

>[!VIDEO](https://video.tv.adobe.com/v/3440406/?learn=on&enablevpops)

## Discussione community

Continua la conversazione nella [discussione](https://adobe.ly/48PRE63) della community Adobe Developers Live.

## Conclusioni principali

* **Introduzione ai componenti Web** I componenti Web consentono agli sviluppatori di creare elementi HTML personalizzati con il proprio aspetto e la propria interattività, definiti mediante JavaScript.
* **Tecnologie di base** I componenti Web vengono creati utilizzando tre tecnologie di base** elementi personalizzati, DOM shadow e modelli HTML.
* **Elementi personalizzati** Gli elementi personalizzati consentono la creazione di nuovi tag HTML. Devono usare kebab-case e includere un trattino. Le classi JavaScript vengono utilizzate per definirne il comportamento.
* **DOM shadow** Il DOM shadow fornisce incapsulamento per la struttura DOM di un componente, impedendo la perdita di CSS e consentendo uno stile più controllato.
* **Modelli HTML** I modelli HTML consentono di definire HTML e CSS che possono essere clonati e aggiunti al DOM. Tuttavia, il relatore preferisce utilizzare gli slot rispetto ai modelli per una migliore distribuzione e flessibilità.
* **Attributi ed eventi** Gli elementi personalizzati possono avere attributi e gestori di eventi, ad esempio connectedCallback e disconnectedCallback, per gestirne il comportamento quando vengono aggiunti o rimossi dal DOM.
* **Gli slot** consentono l&#39;inserimento di contenuto nei componenti Web, supportando sia gli slot predefiniti che quelli denominati per una gestione più flessibile dei contenuti.
* **Esempi reali** Gli esempi includono un visualizzatore di incorporamento di PDF, segnaposto per immagini e un ordinatore di tabelle, che illustrano le applicazioni pratiche dei componenti web.
* **Miglioramento progressivo** I componenti Web possono migliorare le HTML esistenti senza interrompere le funzionalità se JavaScript non viene caricato.
* **Passaggi successivi e risorse** La presentazione suggerisce di esplorare la partecipazione al modulo, il DOM dell&#39;ombreggiatura dichiarativa, gli attributi HTML personalizzati e il rendering lato server. Le risorse includono MDN, webcomponents.org e il libro &quot;Web Components in Action&quot; di Ben Farrell.