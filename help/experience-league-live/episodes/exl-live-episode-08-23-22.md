---
title: 'Chiedi agli esperti: estensioni utili in Tag (Launch) per contribuire a sovrascrivere l’SDK per web'
description: Stai pensando di migrare l’implementazione al nuovo Adobe Web SDK?  Eseguiremo alcune delle nostre estensioni preferite nella libreria Tag di Adobe, che ti aiuteranno a portare la tua raccolta dati al livello successivo.
solution: Data Collection, Experience Platform
feature: Tags
kt: 10528
event-start-time: 2022-08-23 09:00-7
event-guests: Rudi Shumpert,Jeff Chasin,Eric Matisoff
exl-id: 5ef987f4-37f5-473f-b9f2-1598b7e655ba
duration: 3833
source-git-commit: 0b2f63198af8767f24783dbafd244c9398c24f33
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 0%

---

# Domande agli esperti: estensioni utili in Tag (Launch) per contribuire a sovrascrivere il Web SDK

Stai pensando di migrare l’implementazione al nuovo Adobe Web SDK?  Eseguiremo alcune delle nostre estensioni preferite nella libreria Tag di Adobe, che ti aiuteranno a portare la tua raccolta dati al livello successivo.

>[!VIDEO](https://video.tv.adobe.com/v/346610/?quality=12&learn=on)

## Domande e commenti del programma

### Estensione Data Element Assistant da Evolytics

<br> 
**Domanda:** Dal punto di vista della sicurezza dei dati, Evolytics è sicuro da utilizzare, in quanto si tratta di un&#39;estensione di terze parti?

**Risposta:** Sì. Se lo desideri, puoi rivedere il codice dell’estensione, inoltre non salva alcuna data, ma esegue semplicemente una trasformazione.

<br> 

**Domanda:** Questo acquisisce anche l&#39;Adobe ECID?

**Risposta:** l&#39;identificatore ECID di Adobe non viene acquisito all&#39;interno di tale estensione. Questa estensione è destinata alla creazione di identificatori aggiuntivi e anonimi (tra le altre cose).

**Risposta:** L&#39;identificatore ECID Adobe può essere acquisito in altri modi. Lo condivideremo tramite le note e il Twitter ExL poiché non è possibile condividere i collegamenti nella chat qui.

<br> 

**Domanda:** La funzionalità hash offre diverse tecniche di hashing come SHA-256 e fornisce chiavi pubbliche e private?

**Risposta:** Sì! SHA-256 è il valore predefinito

<br> 

### Domande generali e commenti:

<br> 

**Domanda:** Che cosa si fa clic per scaricare i file di origine per le estensioni? È nel &quot;menu a 3 punti&quot;?

**Risposta:** Sì! I 3 punti, quindi Scarica Source (dalla vista catalogo)

<br> 

**Commento:** una delle cose che mi interessano davvero delle estensioni è il loro aspetto che consente di risparmiare tempo. Molte di queste operazioni possono essere eseguite da *1} con un codice personalizzato, ma con un&#39;estensione non è necessario scrivere tale codice.*

**Risposta:** a destra il. Ed è ripetibile senza dover ricreare ogni volta la ruota.

<br> 

**Domanda:** In che modo i plug-in di Analytics saranno supportati o sostituiti con le implementazioni dell&#39;SDK per web?

**Risposta:** molti plug-in di Analytics non sono più necessari in questi giorni grazie alla maggiore flessibilità di Workspace e dei tag Adobe. Tuttavia, quelli che non lo sono, vengono migrati attivamente per l’utilizzo da parte dell’SDK per web.

<br> 

**Domanda:** Sviluppi nel tracciamento di Activity Map tramite Web SDK?

**Risposta:** sono felice di segnalare che l&#39;Activity Map sta lavorando attivamente per il supporto anche in Web SDK

<br> 

**Domanda:** Potremmo avere accesso alla rete Adobe Edge per gestire gli eventi prima di trasferirli alle destinazioni finali? So che possiamo farlo anche in Launch, ma in futuro sarebbe possibile farlo anche al server?

**Risposta:** Sì! Ciò è possibile tramite la funzione di Inoltro eventi, che i clienti possono acquistare tramite qualsiasi prodotto Real-Time CDP (Real-Time CDP Connections, Prime o Ultimate).

**Risposta:** le connessioni RTCDP (Inoltro eventi) consentono di avere maggiore controllo prima di inviarle a destinazioni non adobe.

**Risposta:** Consulta alcuni degli altri video ExL Live per ulteriori informazioni (ad esempio [questo video](exl-live-episode-06-23-22.md)).

<br> 

**Commento:** Chiamata rapida per una delle mie estensioni preferite: esiste un&#39;estensione della tabella di mappatura in cui puoi leggere una tabella per un elemento dati che &quot;se questo valore è questo, impostalo come tale&quot;.

**Risposta:** La flessibilità che offrono è notevole. Inoltre, se lo desiderano, le aziende possono creare anche le proprie estensioni private.

<br> 

**Domanda:** hai mostrato i dati individuali da CRM come città e meteo, quindi dove stiamo memorizzando la risposta individuale?

**Risposta:** le risposte sono memorizzate in ogni evento univoco che attiva una regola all&#39;interno di una proprietà di inoltro eventi e vengono utilizzate solo in tale evento specifico.

<br> 

Continua la discussione su questo argomento nella [discussione della community di Experienci League](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-platform/experience-league-live-post-session-discussion-useful-extensions/m-p/542620#M240).
<br> 

## Experience League aggiuntivo di sessioni LIVE da questa serie di raccolta dati

* [Ask the experts - The basics of Web SDK (Domande agli esperti: nozioni di base di Web SDK)](exl-live-episode-05-26-22.md)
* [Domande agli esperti: connessioni RTCDP](exl-live-episode-06-23-22.md)
* [Domande agli esperti: flussi di dati e preparazione dei dati](exl-live-episode-07-21-22.md)

