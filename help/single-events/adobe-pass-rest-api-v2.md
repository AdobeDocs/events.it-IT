---
title: Adobe Pass - nuova API REST v2
description: Questa sessione si concentra sull’introduzione della nuova API REST v2 di Adobe e su come guidare gli utenti durante il processo di migrazione.
role: Developer
level: Beginner, Intermediate, Experienced
doc-type: Technical Video
duration: 3230
last-substantial-update: 2025-04-07T00:00:00Z
jira: KT-17685
hidefromtoc: true
source-git-commit: 1082d67d49901e151115255b585799a5f57bda4a
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---


# Adobe Pass - nuova API REST v2

Questa sessione si concentra sull’introduzione della nuova API REST v2 di Adobe e su come guidare gli utenti durante il processo di migrazione.

>[!VIDEO](https://video.tv.adobe.com/v/3457461/?learn=on&enablevpops)

## Elementi di rilievo

* **Panoramica e vantaggi**

   * REST API v2 è progettato per un’autenticazione moderna, flessibile e scalabile, in grado di soddisfare eventi ad alta richiesta e scenari multi-dispositivo.
   * I miglioramenti principali includono crittografia avanzata, coerenza delle sessioni, SSO tra dispositivi e informazioni di errore estese per un debug più rapido.

* **Passaggi di migrazione**

   * Gli utenti devono creare nuove applicazioni registrate con ambiti REST API v2.
   * Le configurazioni esistenti come l’identificazione del dispositivo e le mappature MVPD possono essere riutilizzate.
   * La migrazione prevede fasi quali registrazione, configurazione, autenticazione, pre-autorizzazione e autorizzazione.

* **Miglioramenti funzionali**

   * L’API RESTful unificata sostituisce gli SDK di Access Neighbor, semplificando l’implementazione tra le piattaforme.
   * Supporto per più profili di autenticazione all’interno della stessa sessione e transizioni tra dispositivi senza soluzione di continuità.
   * I flussi di pre-autorizzazione e autorizzazione rimangono obbligatori per l’accesso ai contenuti.

* **Timeline**

   * REST API v1 cesserà di ricevere aggiornamenti entro dicembre 2025 e sarà completamente ritirato entro la fine del 2026.
   * Gli utenti sono invitati a completare la migrazione ben prima di queste scadenze.

* **Risorse e supporto**

   * Documentazione, libri di cucina e domande frequenti sono disponibili su Adobe Experience League.
   * Adobe offre ambienti sandbox, ticket Zendesk e riunioni sulla migrazione per il supporto.

* **Elementi di rilievo domande e risposte**

   * REST API v2 richiede la riautenticazione in quanto non è compatibile con le versioni precedenti della v1.
   * La pre-autorizzazione è a scopo di interfaccia utente, mentre l’autorizzazione è necessaria per i token multimediali.
   * SSO è supportato tramite un nuovo token di servizio Adobe.

