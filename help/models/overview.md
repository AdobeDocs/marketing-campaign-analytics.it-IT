---
title: Panoramica dei modelli
description: Scopri come creare, addestrare, valutare e gestire modelli di apprendimento automatico in Marketing Campaign Analytics per misurare e prevedere i risultati di marketing.
feature: Models
exl-id: c43d9bc9-4429-45c2-9247-bd24510a24be
autotag-review: '2026-05-01T08:59:10.903Z'
TQID: 'https://experienceleague.adobe.com/T37YTKQlT1mUIfGkJwQkLLGkP0WfTs6jUbZpskPUHgo'
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Marketing Campaign Analytics
feature_v2:
  - id: a234aebd-3855-4376-a64d-29b38411e0c5
    internal-label: Marketing mix modeling
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
    internal-label: Harmonized data
  - id: f40f1683-8300-4054-aab8-77da06ad63ff
    internal-label: Models
  - id: fe1c9ae8-a908-4ae1-a0b6-fcf35177b134
    internal-label: Marketing touch attribution
subfeature_v2:
  - id: a9505d76-24a1-4ffe-bd01-6ac32d5af453
    internal-label: Model insights
  - id: c89e26b6-808d-4500-8b01-450a63466999
    internal-label: Build model
  - id: cb40363e-1205-4921-971c-9ee6bdb18329
    internal-label: Scoring data
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
    internal-label: Machine learning
source-git-commit: 47233296898cdc0329ff7f43f897c65b4c470ee2
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 0%
---
# Panoramica dei modelli

{{mm-mca-rebranding}}

La funzionalità dei modelli di Marketing Campaign Analytics consente di configurare, addestrare e valutare modelli specifici per gli obiettivi aziendali. La formazione e il punteggio supportano l’apprendimento del trasferimento basato sull’intelligenza artificiale tra attribuzione multitouch e modellazione marketing mix.

I modelli si basano sui dati armonizzati creati come parte del flusso di lavoro dell’applicazione.

Un modello in Marketing Campaign Analytics è un modello di apprendimento automatico utilizzato per misurare e prevedere un risultato specifico basato sugli investimenti di un addetto marketing. I punti di contatto di marketing e i dati di riepilogo possono essere utilizzati come input. Marketing Campaign Analytics consente di creare varianti di modelli basati su diversi set di variabili, dimensioni e risultati, come ricavi, unità vendute, lead.

Un modello richiede:

* Una conversione.
* Uno o più punti di contatto di marketing (canali) costituiti da dati a livello di riepilogo, dati dei punti di contatto di marketing (dati evento) o entrambi.
* Un intervallo di lookback configurabile.
* Una finestra di formazione configurabile.

Un modello può facoltativamente includere:

* Fattori esterni.
* Fattori interni.
* Conoscenza preventiva dei contributi di marketing da altre fonti, come la precedente esperienza delle parti interessate, test incrementali, altri modelli.
* La condivisione di spesa, che utilizza come proxy la condivisione di spesa relativa quando i dati di marketing sono sparsi.

La prima volta che viene creato un modello, la creazione avvia immediatamente il processo di formazione e punteggio. Dopo il completamento dell’esecuzione iniziale dell’addestramento e del punteggio, gli approfondimenti del modello sono disponibili per la revisione. Un modello può essere successivamente riqualificato. Inoltre, i dati possono essere aggiunti al modello che richiede il ripristino manuale del modello. La riqualificazione e il ricalcolo sono un processo iterativo, in quanto emergono nuovi risultati e informazioni e sono necessari adeguamenti per ottenere un adattamento del modello più appropriato per gli obiettivi aziendali.

## Modellazione Full funnel

{{release-limited-testing-section}}

La modellazione completa di funnel consente di modellare le fasi reali del funnel. Ad esempio, dall’iscrizione alla newsletter fino a un acquisto. La modellazione completa di funnel mostra come il marketing sposta i clienti attraverso quel funnel. La modellazione completa di funnel attribuisce il merito ai canali funnel superiori per le conversioni che questi canali influenzano a valle e riconcilia i risultati in modo che i contributi si sommino correttamente senza doppi conteggi.

Puoi utilizzare la modellazione completa di funnel per modellare su un indicatore KPI funnel superiore insieme a un indicatore KPI funnel inferiore.

* Esempi di KPI superiori di funnel sono le iscrizioni a newsletter e altre metriche di brand awareness.
* Esempi di metriche funnel inferiori sono le metriche di conversione tipiche, come ricavi e ordini.

Le tattiche del funnel superiore spesso ottengono meno credito in un modello MMM incentrato sulla conversione. La modellazione completa di funnel consente di comprendere:

* Quali tattiche mediatiche e di marketing hanno contribuito all’obiettivo superiore di funnel.
* Quali tattiche mediatiche e di marketing hanno avuto un impatto indiretto sull’obiettivo di conversione. I pesi massimi del modello funnel sono un input per il modello funnel inferiore per dare maggiore peso ai media e alle tattiche di marketing, se del caso.

## Creare modelli

Per creare un modello, utilizzare il flusso di configurazione guidato passo passo del modello di Marketing Campaign Analytics disponibile quando si seleziona **[!UICONTROL Open model canvas]**. Per ulteriori dettagli, vedi [Modelli di compilazione](build.md).

## Gestisci modelli

Per visualizzare una tabella dei modelli correnti, nell’interfaccia di Marketing Campaign Analytics:

1. Seleziona ![FileDataS2](/help/assets/icons2/FileData.svg) **[!UICONTROL Models]** dalla barra a sinistra.

1. Viene visualizzata una tabella dei modelli correnti.

   Le colonne della tabella specificano i dettagli relativi al modello.

   | Nome colonna | Dettagli |
   |---|---|
   | **[!UICONTROL Name]** | Nome del modello. Se un modello è abilitato per la modellazione completa di funnel, verrà visualizzato un bage di [!BADGE Full funnel]{type=Informative}. |
   | **[!UICONTROL Description]** | Descrizione del modello. |
   | **[!UICONTROL Conversion event]** | Conversione selezionata per il modello. |
   | **[!UICONTROL Run frequency]** | Frequenza di esecuzione dell&#39;addestramento del modello. |
   | **[!UICONTROL Last run]** | La data e l’ora dell’ultimo addestramento del modello. |
   | **[!UICONTROL Status]** | Stato del modello. |

   Per ordinare la tabella in qualsiasi colonna in ordine crescente ![ArrowMoveUpS2](/help/assets/icons2/ArrowMoveUp.svg) o decrescente ![ArrowMoveDownS2](/help/assets/icons2/ArrowMoveDown.svg), selezionare il titolo della colonna.

   Per ordinare o ridimensionare la colonna **[!UICONTROL Name]**, selezionare **[!UICONTROL Name]** ![ChevronDown](/help/assets/icons/ChevronDown.svg). Dal menu di scelta rapida selezionare **[!UICONTROL Sort ascending]**, **[!UICONTROL Sort descending]** o **[!UICONTROL Resize column]**. In alternativa, è possibile passare il puntatore del mouse sul separatore di colonna per ridimensionare la colonna **[!UICONTROL Name]**.

   Lo stato segnalato del modello dipende dalla posizione in cui si trova un modello all&#39;interno del suo ciclo di vita. Ad esempio, se un modello viene creato, o riaddestrato con successo o meno, o ha ottenuto o ottenuto nuovamente un punteggio.

   Nella tabella seguente:

   * ![Segno di spunta](/help/assets/icons/Checkmark.svg): indica la corretta esecuzione di un passaggio del ciclo di vita del modello.
   * ![Orologio](/help/assets/icons/Clock.svg): indica un&#39;esecuzione corrente continua di un passaggio del ciclo di vita del modello.
   * ![Chiudi](/help/assets/icons/Close.svg) - indica una mancata esecuzione di un passaggio nel ciclo di vita del modello.

   | Stato | [Build](/help/models/build.md) | [Addestra](/help/models/train-score.md#train) | [Punteggio](/help/models/train-score.md#score) | [Riprova](/help/models/train-score.md#train) | [Riscore](/help/models/train-score.md#score) |
   |---|:---:|:---:|:---:|:---:|:---:|
   | In corso | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | | | | |
   | In corso | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Orologio](/help/assets/icons/Clock.svg) | | | |
   | In corso | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Orologio](/help/assets/icons/Clock.svg) | | |
   | In corso | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Orologio](/help/assets/icons/Clock.svg) | |
   | In corso | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Orologio](/help/assets/icons/Clock.svg) |
   | Addestramento non riuscito | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Chiudi](/help/assets/icons/Close.svg) | | | |
   | Addestramento non riuscito | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Chiudi](/help/assets/icons/Close.svg) | |
   | Formazione completata | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | | | |
   | Formazione completata | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | |
   | Punteggio non riuscito | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Chiudi](/help/assets/icons/Close.svg) | | |
   | Punteggio non riuscito | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Chiudi](/help/assets/icons/Close.svg) |
   | Punteggio riuscito | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | | |
   | Punteggio riuscito | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) | ![Segno di spunta](/help/assets/icons/Checkmark.svg) |

   {style="table-layout:fixed"}

1. Per modificare le colonne visualizzate per l&#39;elenco, selezionare ![Impostazioni colonna](/help/assets/icons/ColumnSetting.svg) e attivare o disattivare le colonne in ![Controlla](/help/assets/icons/Checkmark.svg).

È possibile eseguire le azioni seguenti su un modello specifico.

### Approfondimenti modello

La funzionalità Approfondimenti modello è disponibile solo su modelli con formazione e punteggi completati.

Per visualizzare le informazioni di un modello:

1. Seleziona ![FileData](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** dalla barra a sinistra.
1. Selezionate il nome del modello.

Sei stato reindirizzato a [Model Insights](insights.md).

### Visualizza dettagli

Per visualizzare ulteriori dettagli su un modello:

1. Seleziona ![FileData](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** dalla barra a sinistra.

1. Seleziona ![Info](/help/assets/icons/Info.svg) per un modello per visualizzare un popup con dettagli come **[!UICONTROL Description]**, **[!UICONTROL Run frequency]**, **[!UICONTROL Last run status]**, **[!UICONTROL Spend share]** e altro ancora.




### Duplica

Potete duplicare rapidamente un modello.

1. Seleziona ![FileData](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** dalla barra a sinistra.

1. Seleziona ![Altro](/help/assets/icons/More.svg) per un modello e dal menu di scelta rapida seleziona **[!UICONTROL Duplicate]**.

Sei stato reindirizzato ai passaggi per creare un nuovo modello, con un nome proposto composto dal nome del modello originale seguito da **[!UICONTROL (Copy)] (_n_)**.

### Modifica

Puoi modificare il nome, la descrizione e la pianificazione dell’apprendimento e del punteggio di un modello.

1. Seleziona ![FileData](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** dalla barra a sinistra.

1. Seleziona ![Altro](/help/assets/icons/More.svg) per un modello e dal menu di scelta rapida seleziona **[!UICONTROL Edit]**.

   Nella finestra di dialogo **[!UICONTROL Edit model]**:

   ![Modifica modello](../assets/model-edit.png)

   * Immettere un nuovo **[!UICONTROL Name]** e **[!UICONTROL Description]**.

   * Per abilitare la pianificazione, abilitare **[!UICONTROL Enable schedule model training and scoring]**. Puoi abilitare la pianificazione solo per i modelli che sono stati addestrati e valutati.

     1. Seleziona **[!UICONTROL Scoring frequency]**:

        * **[!UICONTROL Daily]**: immettere un&#39;ora valida (ad esempio `10:00 am`) oppure utilizzare ![Orologio](/help/assets/icons/Clock.svg) per definire l&#39;ora.
        * **[!UICONTROL Weekly]**: selezionare un giorno della settimana e immettere un&#39;ora valida (ad esempio `10:00 am`) oppure utilizzare ![Orologio](/help/assets/icons/Clock.svg) per definire l&#39;ora.
        * **[!UICONTROL Monthly]**: selezionare un giorno del mese dal menu a discesa Esegui su ogni e immettere un&#39;ora valida (ad esempio `10:00 am`) oppure utilizzare ![Orologio](/help/assets/icons/Clock.svg) per definire l&#39;ora.

     1. Selezionare **[!UICONTROL Training frequency]** dal menu a discesa: **[!UICONTROL Monthly]**, **[!UICONTROL Quarterly]**, **[!UICONTROL Yearly]** o **[!UICONTROL None]**.

   * Per aggiornare i campi di reporting di [granular insights](/help/models/build.md#granular-insights-reporting-fields), nella sezione **[!UICONTROL Granular Insights Reporting Fields]**:
     1. Seleziona uno o più campi armonizzati da **[!UICONTROL _Seleziona campi armonizzati_]** sotto **[!UICONTROL Includes]**. I campi armonizzati selezionati vengono aggiunti al pannello.
     1. Selezionare **[!UICONTROL *Campo armonizzato *]**![CrossSize100](/help/assets/icons/CrossSize100.svg) per rimuovere un campo armonizzato dal contenitore con i campi armonizzati selezionati.
     1. Selezionare **[!UICONTROL Clear all]** per rimuovere tutti i campi armonizzati selezionati.

     >[!IMPORTANT]
     >Qualsiasi modello con MTA creato prima del 12 gennaio 2026 deve essere duplicato per abilitare informazioni granulari sul modello.<br/>
     >La registrazione è necessaria affinché qualsiasi modello esistente rifletta le dimensioni granulari aggiornate nei dati di punteggio.
     >

1. Seleziona **[!UICONTROL Save]**.

### Addestra

Conserva un modello quando desideri includere nuovi dati di marketing e di fattore incrementali. Per ulteriori informazioni, vedere [Modelli di addestramento e valutazione](train-score.md#train).

### Punteggio

Puoi assegnare un punteggio incrementale a un modello in base a nuovi dati di marketing o ripristinare un modello per un intervallo di date specifico. Per ulteriori informazioni, vedere [Modelli di addestramento e valutazione](train-score.md#score).

### Elimina modelli

Per eliminare un modello:

1. Seleziona ![FileData](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** dalla barra a sinistra.
1. Seleziona ![Altro](/help/assets/icons/More.svg) per un modello e dal menu di scelta rapida seleziona **[!UICONTROL Delete]**. In alternativa, selezionare ![Elimina](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** dalla barra delle azioni blu.
1. Selezionare **[!UICONTROL Delete]** nella finestra di dialogo di conferma **[!UICONTROL Delete model]** per eliminare il modello. Selezionare **[!UICONTROL Cancel]** per annullare.

Per eliminare più modelli:

1. Seleziona più modelli.
1. Dalla barra blu delle azioni, seleziona ![Elimina](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** per eliminare i modelli.
1. Selezionare **[!UICONTROL Delete]** nella finestra di dialogo di conferma **[!UICONTROL Delete *x *modelli]**&#x200B;per eliminare i modelli. Selezionare **[!UICONTROL Cancel]**&#x200B;per annullare.

