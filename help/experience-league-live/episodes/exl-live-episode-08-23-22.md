---
title: 'Chiedi agli esperti: estensioni utili in Tag (Launch) per contribuire a sovrascrivere l’SDK per web'
description: Stai pensando di migrare l’implementazione al nuovo Adobe Web SDK?  Eseguiremo alcune delle nostre estensioni preferite nella libreria Tag di Adobe, che ti aiuteranno a portare la tua raccolta dati al livello successivo.
solution: Data Collection,Experience Platform
kt: 10528
thumbnail: https://video.tv.adobe.com/v/346610?format=jpeg
event-start-time: 2022-08-23 09:00-7
event-cta-url: null
event-guests: Rudi Shumpert,Jeff Chasin,Eric Matisoff
exl-id: 5ef987f4-37f5-473f-b9f2-1598b7e655ba
source-git-commit: 3d2289642f4164bf82dc1c8a42c5798e9183188b
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Domande agli esperti: estensioni utili in Tag (Launch) per contribuire a sovrascrivere il Web SDK

Stai pensando di migrare l’implementazione al nuovo Adobe Web SDK?  Eseguiremo alcune delle nostre estensioni preferite nella libreria Tag di Adobe, che ti aiuteranno a portare la tua raccolta dati al livello successivo.

>[!VIDEO](https://video.tv.adobe.com/v/346610/?quality=12&learn=on)

## Domande e commenti del programma

### Estensione Data Element Assistant da Evolytics

<br> 
**Domanda:** Dal punto di vista della sicurezza dei dati, Evolytics è sicuro da utilizzare, in quanto si tratta di un’estensione di terze parti?

**Risposta:** Sì. Se lo desideri, puoi rivedere il codice dell’estensione, inoltre non salva alcuna data, ma esegue semplicemente una trasformazione.

<br> 

**Domanda:** Questo acquisisce anche l’Adobe ECID?

**Risposta:** L’ECID di Adobe non viene acquisito all’interno di tale estensione. Questa estensione è destinata alla creazione di identificatori aggiuntivi e anonimi (tra le altre cose).

**Risposta:** Tuttavia, l’ECID Adobe può essere acquisito in altri modi. Lo condivideremo tramite le note ExL e Twitter poiché non è possibile condividere i collegamenti nella chat qui.

<br> 

**Domanda:** La funzionalità di hashing offre diverse tecniche di hashing come SHA-256 e fornisce chiavi pubbliche e private?

**Risposta:** Sì! SHA-256 è il valore predefinito

<br> 

### Domande generali e commenti:

<br> 

**Domanda:** Cosa facciamo clic per scaricare i file sorgente per le estensioni? È nel &quot;menu a 3 punti&quot;?

**Risposta:** Sì! I 3 punti, quindi Scarica origine (dalla vista catalogo)

<br> 

**Commento:** Una delle cose che mi interessano davvero delle estensioni è l&#39;aspetto che consente di risparmiare tempo. Molti di loro fanno cose che tu fai *potrebbe* esegui con un codice personalizzato, ma con un’estensione non è necessario scrivere tale codice.

**Risposta:** Proprio così. Ed è ripetibile senza dover ricreare ogni volta la ruota.

<br> 

**Domanda:** Come verranno supportati o sostituiti i plug-in di Analytics con le implementazioni dell’SDK per web?

**Risposta:** Al giorno d’oggi, molti plug-in di Analytics sono effettivamente superflui grazie alla maggiore flessibilità di Workspace e dei tag Adobe. Tuttavia, quelli che non lo sono, vengono migrati attivamente per l’utilizzo da parte dell’SDK per web.

<br> 

**Domanda:** Sviluppi sul tracciamento di Activity Map con Web SDK?

**Risposta:** Sono felice di segnalare che l’Activity Map sta attivamente lavorando per il supporto anche in Web SDK

<br> 

**Domanda:** Potremmo avere accesso alla rete Adobe Edge per gestire gli eventi prima di trasferirli alle destinazioni finali? So che possiamo farlo anche in Launch, ma in futuro sarebbe possibile farlo anche al server?

**Risposta:** Sì! Ciò è possibile tramite la funzione di Inoltro eventi, che i clienti possono acquistare tramite qualsiasi prodotto Real-Time CDP (Real-Time CDP Connections, Prime o Ultimate).

**Risposta:** Connessioni RTCDP (Inoltro eventi) consente di avere un maggiore controllo prima di inviarlo a destinazioni non adobe.

**Risposta:** Guarda alcuni degli altri video ExL Live per saperne di più su questo (come [questo](exl-live-episode-06-23-22.md)).

<br> 

**Commento:** Chiamata rapida per una delle mie estensioni preferite: esiste un’estensione della tabella di mappatura in cui puoi leggere una tabella per un elemento dati che &quot;se questo valore è questo, impostalo come tale&quot;.

**Risposta:** La flessibilità che offrono è impressionante. Inoltre, se lo desiderano, le aziende possono creare anche le proprie estensioni private.

<br> 

**Domanda:** Hai mostrato i dati individuali di gestione delle relazioni con i clienti come città e meteo, dove stiamo memorizzando la risposta individuale?

**Risposta:** Le risposte vengono memorizzate in ogni evento univoco che attiva una regola all&#39;interno di una proprietà di Inoltro eventi e vengono utilizzate solo in tale evento specifico.

<br> 

Continua la discussione su questo argomento in [Experience League discussione della community](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-platform/experience-league-live-post-session-discussion-useful-extensions/m-p/542620#M240).
<br> 

## Experience League aggiuntivo di sessioni LIVE da questa serie di raccolta dati

* [Ask the experts - The basics of Web SDK (Domande agli esperti: nozioni di base di Web SDK)](exl-live-episode-05-26-22.md)
* [Domande agli esperti: connessioni RTCDP](exl-live-episode-06-23-22.md)
* [Domande agli esperti: flussi di dati e preparazione dei dati](exl-live-episode-07-21-22.md)
