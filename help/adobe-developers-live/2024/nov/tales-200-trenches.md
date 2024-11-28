---
title: Racconti da 200 trincee
description: Assicurati il successo del progetto web dando priorità alle prestazioni, utilizzando Google PageSpeed Insights, ottimizzando metriche chiave come LCP e TBT, gestendo le risorse in modo efficiente e seguendo le best practice per lo sviluppo e l’ottimizzazione delle immagini.
solution: Experience Manager, Experience Manager Sites
feature: Edge Delivery Services
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1321
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16541
source-git-commit: 07d4174b0d89ba2c417866e76ae72f015b91b03a
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# Racconti da 200 trincee

Con oltre 200 Edge Delivery Services di progetti completati, Kiran Murugulla, Senior Engineer presso Adobe, e Varun Mitra, Architetto per Adobe Experience Manager Cloud, condividono le principali lezioni apprese. Scopri i segreti che si nascondono dietro la distribuzione di esperienze veloci e ad alte prestazioni con core Web Vitals eccezionali.


>[!VIDEO](https://video.tv.adobe.com/v/3439424/?learn=on&enablevpops)

## Discussione community

Continua la conversazione nella [discussione](https://adobe.ly/4fwWvvi) della community Adobe Developers Live.

## Punti chiave da eliminare

* **Le prestazioni sono critiche** Le prestazioni, in particolare la velocità delle pagine Web, sono un fattore chiave per il successo dei progetti Web. Garantire punteggi di prestazioni pari a 100 è un obiettivo primario.
* **Procedure di sviluppo**
   * Utilizza Google PageSpeed Insights per eseguire test continui durante lo sviluppo.
   * Avvia i progetti con un codice boilerplate che ha già un punteggio di 100 per mantenere alte le prestazioni.
   * Prima dell’unione, assicurati che le richieste pull (PR) soddisfino gli standard di prestazioni.
* **Metriche chiave** si concentrano sull&#39;ottimizzazione di LCP (Largest Contentful Paint) e TBT (Total Blocking Time) in quanto influiscono in modo significativo sui punteggi delle prestazioni.
* **Gestione risorse**
   * Includi le risorse necessarie, come font e script di terze parti, nell’origine del progetto.
   * Utilizza i fallback dei font per migliorare i tempi di caricamento.
   * Ritarda il caricamento di script non essenziali per migliorare le prestazioni di caricamento iniziali.
* **Ottimizzazione immagine** Assegna la priorità al caricamento di immagini superiori alla piega e utilizza le impostazioni di recupero ad alta priorità per le immagini critiche.
* **Casi di studio**
   * ***CNN.com*** ha ottimizzato gli indici di query e ha ritardato il caricamento degli annunci Google per migliorare le prestazioni.
   * ***Herbert Homes*** ha utilizzato l&#39;API Intersection Observer per caricare i dati mentre gli utenti scorrono, migliorando le prestazioni e l&#39;esperienza utente.
* **Best practice**
   * Inizia con un codice boilerplate e utilizza un markup ben strutturato.
   * Utilizza selettori CSS avanzati e riduci al minimo la manipolazione del JavaScript.
   * Concentrati sullo sviluppo mobile-first.
   * Garantire agli autori una struttura dei contenuti intuitiva.
* **Strumenti** Utilizza strumenti come Google Sheets e DSA per tenere traccia dei punteggi delle prestazioni del sito nel tempo.

