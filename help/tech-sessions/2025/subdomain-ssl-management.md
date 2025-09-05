---
title: 'Sessioni tecniche: sottodominio Adobe Campaign e gestione SSL nel Pannello di controllo Campaign'
description: Scopri come delegare e configurare i sottodomini nel Pannello di controllo Campaign di Adobe Campaign, configurare i certificati SSL e monitorare la configurazione per garantire il recapito sicuro delle e-mail.
solution: Campaign
feature: Subdomains and Certificates
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3409
last-substantial-update: 2025-09-05T00:00:00Z
jira: KT-18866
source-git-commit: 18ce421793d97372198151afc92b24f3bed053a8
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Sessioni tecniche: Sottodominio Adobe Campaign e gestione SSL nel Pannello di controllo Campaign

In questa sessione esploriamo i concetti di delega e configurazione dei sottodomini all’interno di Adobe Campaign, inclusa l’installazione di certificati SSL nei sottodomini protetti.

Scopri cos’è un sottodominio, i suoi scopi e i metodi di delega che consentono ad Adobe di utilizzarlo in modo efficace. La sessione illustra inoltre i principi per la protezione di un sottodominio tramite certificati SSL e le best practice per mantenere un ambiente sicuro.

Forniamo indicazioni dettagliate sulla configurazione dei sottodomini utilizzando il Pannello di controllo Campaign self-service, evidenziando i potenziali ostacoli e come affrontarli. I partecipanti acquisiscono conoscenze pratiche per garantire una configurazione fluida e una gestione sicura dei loro sottodomini.

Che tu sia un amministratore, uno sviluppatore o un proprietario di piattaforma, questa sessione ti offre le competenze necessarie per configurare e proteggere in modo sicuro i sottodomini in Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3471391/?learn=on&enablevpops)

## Gestione dei sottodomini in Adobe Campaign

Sblocca le funzionalità di base di delega, configurazione e sicurezza dei sottodomini per le comunicazioni e-mail di Adobe Campaign:

* **Delega dei sottodomini** Scegli tra delega completa o CNAME per controllare il modo in cui Adobe gestisce il recapito messaggi DNS ed e-mail.
* **Configurazione DNS e SSL** La corretta configurazione dei certificati MX, SPF, DKIM, DMARC e SSL è fondamentale per un invio di e-mail sicuro e affidabile.
* **Pannello di controllo Campaign** Utilizza lo strumento self-service di Adobe per semplificare la configurazione del sottodominio, monitorare i record e gestire i certificati SSL.
* **Insidie comuni** Per evitare ritardi ed errori, consulta le tempistiche di controllo, i requisiti dei record e i passaggi per la risoluzione dei problemi.

La padronanza di questi processi garantisce che le campagne siano sicure, consegnabili e che la reputazione del tuo marchio sia preservata.

## Metodi di delega** Full vs. CNAME

* **Delega completa** Adobe gestisce tutti i record DNS per il sottodominio, garantendo recapito messaggi e sicurezza ottimali. Consigliato per la maggior parte degli utenti.
* **Delega CNAME** Il cliente e Adobe condividono le responsabilità DNS. Il cliente crea record CNAME che puntano alle risorse gestite da Adobe.
* **Differenze chiave:
* **Full** Adobe ha piena autorità; meno manutenzione clienti.
* **CNAME** ha condiviso la responsabilità; ulteriori passaggi manuali per il cliente.
* **Suggerimento** Non delegare mai il dominio radice, solo i sottodomini, per evitare di perdere il controllo sul dominio principale.
