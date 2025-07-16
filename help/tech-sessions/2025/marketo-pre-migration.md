---
title: Migrazione di Marketo a Adobe Admin Console - (pre-migrazione)
description: Adobe sta eseguendo la migrazione di Marketo Engage ad Admin Console per migliorare la gestione degli utenti. Scopri i tipi di migrazione automatica e automatica, i prerequisiti, le modifiche successive alla migrazione, le best practice, le insidie comuni e il supporto. Accedi alla registrazione della sessione sul sito web Experience League di Adobe.
solution: Marketo Engage
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 2280
last-substantial-update: 2025-03-14T00:00:00Z
jira: KT-17483
exl-id: 9c3da83f-9e02-4a2e-9784-10213facf056
source-git-commit: 088615f28aa91dfd4ba119c11c4c9f8a89441d84
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Migrazione di Marketo a Adobe Admin Console: pre-migrazione

Unisciti a noi per una migrazione diretta a Marketo con gli esperti di Adobe!

Vai al passo con la migrazione a Marketo con il team Customer Experience &amp; Identity di Adobe in questo webinar informativo. Seguirai i passaggi chiave, le best practice e le sfide comuni per garantire una transizione senza problemi a Adobe Admin Console.

Cosa imparerai,

* Una roadmap dettagliata per il processo di pre-migrazione
* Best practice per semplificare la transizione ed evitare malfunzionamenti
* Risposte degli esperti ai problemi comuni relativi alla migrazione

Che tu stia iniziando la migrazione o preparandoti per i passaggi finali, questa sessione ti fornirà le conoscenze e gli strumenti necessari per navigare nel processo con sicurezza. Non perdere questa opportunità per andare avanti e rendere la migrazione Marketo fluida!

>[!VIDEO](https://video.tv.adobe.com/v/3449712/?learn=on&enablevpops)

## Punti chiave da eliminare

### Finalità della migrazione e panoramica

Adobe sta eseguendo la migrazione di Marketo Engage ad Admin Console per consolidare tutti i prodotti in un unico hub per migliorare la gestione degli utenti e l’accesso.  Admin Console fungerà da hub centrale per la gestione dei prodotti Adobe, dei ruoli utente, delle autorizzazioni e dell’accesso al supporto. Gli URL per accedere a Marketo Engage passeranno alla piattaforma Experience Cloud di Adobe.

### Tipi di migrazione

* **Migrazione automatica** per le organizzazioni con meno di 75 utenti e nessuna configurazione SSL. Adobe gestisce la migrazione.
* **Migrazione automatica** per le organizzazioni con configurazione SSL. Gli amministratori gestiscono il processo di migrazione utilizzando la console di migrazione.

### Prerequisiti per la migrazione

* Gli amministratori di sistema devono completare l’e-mail di consenso.
* SSL deve essere impostato in Admin Console (non nell’istanza Marketo).

### Modifiche post-migrazione

* Gli utenti accederanno utilizzando Adobe ID o Federated ID (SSL).
* I ruoli e le autorizzazioni amministratore determineranno i livelli di accesso in Admin Console.

### Best practice

* Verifica le e-mail degli utenti e risolvi gli account bloccati prima della migrazione.
* Assicurati di assegnare i ruoli di amministratore appropriati.
* Disattiva gli ad blocker o utilizza la modalità di navigazione in incognito per evitare problemi di accesso.

### Insidie comuni

* Autorizzazioni di amministrazione errate possono limitare l’accesso.
* Le estensioni del browser e gli ad blocker possono interferire con l’accesso.
* L’inserimento di IP nella whitelist non è ancora supportato in Admin Console, ma è in fase di sviluppo.

### Impatto sulla funzionalità

* La migrazione non influirà su e-mail automatizzate, utenti API e codici munchkin.
* La migrazione ha un impatto principalmente sull’autenticazione e la gestione degli utenti.

### Supporto

* Gli utenti che riscontrano problemi devono aprire un caso di supporto con l’Assistenza clienti di Adobe.
* Includi l’ID organizzazione IMS nei casi di supporto per una risoluzione più rapida.
