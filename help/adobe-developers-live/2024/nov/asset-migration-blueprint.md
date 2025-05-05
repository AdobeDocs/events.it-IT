---
title: Blueprint per la migrazione ad Assets
description: Scopri come migrare un DAM legacy ad Adobe Experience Manager Assets con le informazioni provenienti da Achim Koch, che includono analisi delle parti interessate, pianificazione delle risorse, trasformazione dei dati e best practice come l’utilizzo di file CSV per la gestione dei dati.
feature: Migration
topic: Migration
solution: Experience Manager, Experience Manager Assets
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1690
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16576
exl-id: f588055b-05c7-44df-be67-799a0e3ee1ed
source-git-commit: 946d7cd484e8c5d4358d4099b3518705cab8d4a3
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Blueprint per la migrazione ad Assets

Unisciti a Achim Koch, Principal Technical Architect di Adobe, per scoprire come migrare un DAM legacy ad Adobe Experience Manager Assets. Ottieni informazioni sull’analisi delle parti interessate, la pianificazione delle risorse, la trasformazione dei dati e best practice come l’utilizzo di file CSV per la gestione dei dati. Crea una roadmap per i tuoi progetti di migrazione Adobe Experience Manager.

>[!VIDEO](https://video.tv.adobe.com/v/3440447/?learn=on&enablevpops&captions=ita)

## Discussione community

Continua la conversazione nella [discussione](https://adobe.ly/4hKHpnF) della community Adobe Developers Live.

## Punti chiave da eliminare

* **Nessun strumento predefinito per la migrazione** Non esiste un singolo strumento in grado di migrare da vari sistemi legacy a Adobe Experience Manager (AEM) a causa della diversità di prodotti e soluzioni personalizzate.

* **Cinque fasi della migrazione**

   * Pianificazione del progetto
   * Pianificazione dell’implementazione
   * Implementazione AEM
   * Implementazione script di migrazione
   * Esecuzione della migrazione

* **Coinvolgimento delle parti interessate** È fondamentale identificare e coinvolgere le parti interessate quali sponsor, utenti aziendali, amministratori di sistemi IT e supporto di sistemi legacy.

* **Pianificazione delle risorse e della sequenza temporale** Assicurati che le risorse siano disponibili e pianifica le festività, i picchi di orario di lavoro e le finestre off-limit.

* **Pianificazione tecnica** Questo include analisi dei requisiti, trasformazione dei dati e pianificazione dell&#39;infrastruttura.

* **Processo iterativo** La migrazione comporta più iterazioni di esecuzione, analisi, feedback e adattamento degli script.

* **L&#39;utilizzo di file CSV** è preferibile per la facilità d&#39;uso e la leggibilità durante il processo di migrazione.

* **Node.js per il linguaggio script** è consigliato per il supporto di CSV, AWS e HTTP e per offrire una buona opportunità di imparare a utilizzare JavaScript.

* **Qualità e ripetibilità** Garantire una migrazione dei dati di alta qualità, conservare i dati originali e i file CSV come riferimento e rendere il processo ripetibile.

* **Blocco contenuto** Dichiarare un blocco del contenuto durante la migrazione per impedire l&#39;aggiunta di nuovi dati dopo l&#39;acquisizione dello snapshot.

* **Strumenti e suggerimenti** Utilizza strumenti come VS Code con l&#39;estensione CSV Rainbow e considera il delimitatore di ordine dei byte (BOM) per i file di testo UTF-8.

* **Approvazione aziendale** Per rimuovere il blocco dei contenuti, riservare tempo per testare e ottenere l&#39;approvazione aziendale ufficiale dopo la migrazione.
