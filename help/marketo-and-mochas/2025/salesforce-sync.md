---
title: Marketo e Mochas - Sincronizzazione Salesforce
description: Padroneggia la sincronizzazione Marketo-Salesforce con indicazioni esperte su autorizzazioni, visibilità sul campo, collaborazione tra amministratori e best practice per garantire un’integrazione fluida e ottimizzata.
feature: Salesforce Integration
topic: Integrations
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3547
last-substantial-update: 2025-08-07T00:00:00Z
jira: KT-18706
source-git-commit: bc5752512fb1bc50cefe0180c308574e821888a2
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---


# Marketo e Mochas: sincronizzazione Salesforce

Marketo dispone di pochissime integrazioni native, ma Salesforce è la più potente di tutte. Con circa il 90% dei clienti Marketo che utilizzano anche Salesforce, Adobe si impegna a consigliare i clienti su come teorizzare, diagnosticare e ottimizzare la sincronizzazione tra i due. La sincronizzazione di Marketo con SFDC si basa in gran parte sulle autorizzazioni in SFDC concesse all’utente di Marketo Sync. Questo può essere difficile per i clienti a causa di più amministratori o team diversi che creano silos nella comunicazione sugli aggiornamenti nel sistema.

Questo webinar tratta i seguenti argomenti in relazione alla &lt;-> sincronizzazione di Marketo con SFDC:

· Spiegazione del funzionamento della sincronizzazione
· Nascondere campi e oggetti dall&#39;utente di Marketo Sync in SFDC
· Come comunicare con l’amministratore di SFDC
· Come lavorare in modo efficace con il supporto Marketo
· Aspetti da evitare durante la sincronizzazione di Marketo con SFDC

>[!VIDEO](https://video.tv.adobe.com/v/3470624/?learn=on&enablevpops)

## Best practice per l’utilizzo di Salesforce Sync

Per utilizzare Salesforce Sync con Marketo in modo efficace, segui queste best practice, spiegate passo dopo passo in termini semplici:

1. **Comprendere il processo di sincronizzazione**

   La sincronizzazione collega Marketo e Salesforce, consentendo il flusso dei dati tra i due sistemi. Pensa a &quot;Utente di Marketo Sync&quot; come a un ponte tra le due piattaforme. Questo utente dispone delle autorizzazioni per la lettura e la scrittura di determinati dati:

   * **Accesso in scrittura** lead e contatti (Marketo può aggiornarli in Salesforce).
   * **Accesso in lettura** Account, opportunità, oggetti personalizzati e attività (Marketo può visualizzarli ma non modificarli).

   Quando i dati vengono modificati in Salesforce o Marketo, la sincronizzazione aggiorna l&#39;altro sistema ogni cinque minuti. Tuttavia, puoi assegnare la priorità agli aggiornamenti urgenti utilizzando passaggi di flusso come &quot;Sincronizza con SFDC&quot;.

1. **Pulisci campi**

   Sincronizza solo i campi utilizzati attivamente. Ad esempio:

   * Se sono presenti campi obsoleti come &quot;note COVID-19&quot; che non sono più rilevanti, rimuoverli dalla sincronizzazione. Questo riduce il disordine e accelera il processo.
   * Evita di sincronizzare i campi della formula (ad esempio, &quot;lead age in giorni&quot;) perché non aggiornano i timestamp, il che può causare problemi.

1. **Impedisci backlog**

   Si verifica un backlog quando la quantità di dati in attesa di sincronizzazione è eccessiva. Per evitare questo problema:

   * Limita aggiornamenti non necessari: ad esempio, se il punteggio di un account cambia leggermente (ad esempio, da 60 a 61), può attivare gli aggiornamenti per tutti i contatti correlati. Per ridurre gli aggiornamenti, raggruppa i punteggi in intervalli (ad esempio, 0-25, 26-50).
   * Campagne batch: utilizza campagne batch invece di attivare campagne per elaborare i dati in modo più efficiente.

1. **Gestisci errori**

   Possono verificarsi errori quando Marketo tenta di aggiornare un campo in Salesforce ma non dispone dell’autorizzazione. Per risolvere i problemi:

   * Accedi a Salesforce come utente Marketo Sync e prova ad eseguire la stessa azione. Questo aiuta a identificare i problemi di autorizzazione o i dati non validi.
   * Imposta campagne ricorrenti in Marketo per correggere errori comuni, come la standardizzazione dei valori paese/stato (ad esempio, da &quot;CA&quot; a &quot;California&quot;).

1. **Usa filtri di sincronizzazione personalizzati**

   I filtri personalizzati consentono di controllare quali record sincronizzare tra Salesforce e Marketo. Ad esempio, crea un campo denominato &quot;Do Not Sync to Marketo&quot; (Non sincronizzare con). Se questo campo è contrassegnato come &quot;true&quot; per un record, non verrà sincronizzato con Marketo. Ciò è utile per escludere indirizzi e-mail non validi o contatti obsoleti.

1. **Limita creazione attività**

   Elm Salesforce. Concentrati su attività significative, come &quot;modulo compilato&quot; o &quot;collegamento cliccato nell’e-mail&quot;.

1. **Collabora con il tuo amministratore Salesforce**

   Poiché la sincronizzazione coinvolge entrambi i sistemi, rivolgiti al tuo amministratore Salesforce per:

   * Gestisci le autorizzazioni per l&#39;utente di Marketo Sync.
   * Pulisci i campi non necessari in Salesforce.
   * Risolvere insieme i problemi di sincronizzazione.

1. **Monitora prestazioni sincronizzazione**

   Controlla regolarmente lo stato di sincronizzazione nella sezione amministrazione di Marketo:

   Cerca i picchi nelle dashboard &quot;Tendenza backlog di sincronizzazione&quot; o &quot;Throughput di sincronizzazione&quot;. Ciò indica ritardi o aggiornamenti eccessivi.
Se noti dei problemi, individua i campi o i record che causano il problema.

1. **Utilizzare Gli Oggetti Personalizzati In Modo Saggio**

   Gli oggetti personalizzati sono strutture di dati speciali che possono memorizzare informazioni aggiuntive (ad esempio, dettagli del prodotto). Sincronizza solo gli oggetti personalizzati necessari per le campagne per evitare il gonfiore del database.

1. **Pianificazione per la scalabilità**

   Quando si imposta la sincronizzazione, considerare a lungo termine:

   * Gestisci un dizionario dati per tenere traccia dei campi sincronizzati e perché.
   * Evita di sincronizzare campi o record non necessari per mantenere efficiente il sistema.

Seguendo questi passaggi, puoi garantire un’integrazione fluida ed efficiente tra Marketo e Salesforce, riducendo al minimo gli errori e massimizzando il valore dei dati.
