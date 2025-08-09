---
title: Navigazione semplice nell’API Workfront e nelle modifiche di Fusion per i campi a selezione multipla
description: Scopri le prossime modifiche all’API di Adobe Workfront e a Fusion, inclusi gli aggiornamenti per più campi selezionati, il controllo delle versioni degli abbonamenti agli eventi e le strategie per evitare di interrompere le modifiche.
feature: Workfront API, Workfront Fusion, Workfront Integrations and Apps
topic: Integrations
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3172
last-substantial-update: 2025-08-08T00:00:00Z
jira: KT-18631
source-git-commit: 6225f36c5d26ecca5ebc2aca24a2d592a3279570
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---


# Navigazione semplice nell’API Workfront e nelle modifiche di Fusion per i campi a selezione multipla

Questo workshop è stato registrato il 25 giugno 2025 e ha visto la partecipazione di Andy Hess, che ha condiviso le imminenti modifiche all’API Workfront e a Fusion.

>[!VIDEO](https://video.tv.adobe.com/v/3469978/?learn=on&enablevpops)

## Risorse

Oltre alla registrazione on-demand, abbiamo incluso la presentazione e risorse aggiuntive:
* [Presentazione diapositive PDF](https://workfront-experience.s3.us-west-2.amazonaws.com/Training/Guides/Customer+Success+at+Scale/Navigating+the+API+and+Fusion+Changes+for+Multi-Select+Fields+with+Ease+062425.pdf)
* Un evento ospitato in partnership con il team di sviluppo software Adobe è stato consegnato all&#39;inizio di maggio sulle modifiche apportate alle sottoscrizioni di eventi per ulteriori informazioni su quell&#39;area specifica, [[Follow-up evento] Preservare gli scenari di fusione durante l&#39;aggiornamento V2 delle sottoscrizioni di eventi](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-preserving-your-fusion-scenarios-during-the/m-p/754182#M4041)

## Principali soluzioni e risorse

* Le modifiche ai campi a selezione multipla dell’API Workfront sono disponibili nella versione 21 (ottobre 2025) per garantire la coerenza del formato di array JSON invece di risposte miste stringa/array
* È in corso l&#39;introduzione del controllo delle versioni degli abbonamenti agli eventi: la versione 2 restituirà sempre i campi a selezione multipla come array, mentre la versione 1 manterrà il comportamento incoerente corrente
* Per impostazione predefinita, i nuovi abbonamenti agli eventi vengono impostati sulla versione 2 e tutti gli abbonamenti verranno automaticamente aggiornati alla versione 2 a metà gennaio 2026
* Nel corso dell’anno verrà rilasciata una nuova versione del connettore Workfront con processo di aggiornamento manuale per mantenere la mappatura del modulo ed evitare modifiche che causino interruzioni
* L’assistente di Fusion AI è attualmente disponibile, ma richiede un accordo di IA firmato e una configurazione di licenza appropriata. Per maggiori informazioni, contatta il tuo Account Manager. [Ulteriori informazioni sull&#39;utilizzo di IA in Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/manage-scenarios/fusion-ai-assistant)
* [Modelli di Workfront Fusion attualmente disponibili](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/create-and-manage-templates/currently-available-fusion-templates)
* [Richiama modelli Fusion](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/call-for-fusion-template-ideas/m-p/732085#M3686)- se hai suggerimenti per nuovi modelli Fusion, aggiungili qui. Da qui il team riceve le idee  

Se hai altre domande, rispondi a questo [post della community Experience League](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-navigating-the-workfront-api-and-fusion-changes/td-p/761253). 

Ci auguriamo di incontrarti ai futuri workshop per il successo dei clienti.  Assicurati di estrarre l&#39;[Eventi Workfront](https://experienceleague.adobe.com/events/?filters=Workfront) su Experience League per l&#39;elenco completo e per registrarti.