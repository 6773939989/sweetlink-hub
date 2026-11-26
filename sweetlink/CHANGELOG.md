# Novità

Questo è il testo che Home Assistant mostra quando propone un aggiornamento. Una voce per versione,
la più recente in cima, scritta per chi ha l'impianto in casa e non per chi lo sviluppa.

## 0.1.67

- Il registro di Sweetlink dice anche per Alexa, come già per Google, quando manca l'elenco dei
  dispositivi per i comandi vocali, e quando torna.

## 0.1.66

- I comandi vocali con Alexa usano ora l'elenco dei dispositivi preparato dal sistema Sweetplace, lo
  stesso di Google.
- Sweetlink controlla da solo che Home Assistant sappia dove trovare i dispositivi per Alexa e Google, e se
  qualcosa manca lo sistema e riavvia Home Assistant una volta. Così un file mancante non impedisce più a
  Home Assistant di ripartire.

## 0.1.65

- Con Alexa collegato, l'app Alexa vede subito quando un dispositivo cambia stato, anche se lo accendi
  dall'interruttore o con Google. I dispositivi che aggiungi o togli ai comandi vocali compaiono o spariscono
  in Alexa da soli, senza dover chiedere «Alexa, cerca dispositivi».

## 0.1.64

- L'assistenza di Sweetplace può aggiornare le integrazioni che hai installato con HACS alla versione provata da
  Sweetplace, tenendo una copia di quella di prima. Home Assistant si riavvia una volta sola, alla fine, se almeno una
  integrazione è cambiata o potrebbe esserlo.

## 0.1.63

- Prima parte del collegamento con Alexa: Sweetlink sa passare a Home Assistant i comandi che arrivano da Alexa
  attraverso Sweetplace, e rimandare la risposta. È in prova e non è ancora disponibile nell'app Alexa: niente
  cambia finché la skill di Sweetplace non viene pubblicata.
- I dispositivi scelti per Alexa vengono presentati in italiano. Il cambio si applica al prossimo riavvio di
  Home Assistant.
- Se i dispositivi scelti per Alexa sono più di 300, il massimo che Amazon accetta, Sweetlink ne presenta i primi
  300 e lo scrive nel suo registro.

## 0.1.62

- Dopo il passaggio dello Z-Wave alla copia di Sweetplace, la copia riparte da sola a ogni riavvio dell'impianto,
  anche quando l'add-on del suo autore era impostato per partire a mano.
- L'add-on dell'autore resta installato e fermo come copia di sicurezza, ma non compare più nel menu laterale di
  Home Assistant e il sistema non prova più a riavviarlo da solo: acceso accanto alla copia, si contenderebbe con lei
  la stessa chiavetta Z-Wave. Con «Ripristina» l'assistenza gli rimette tutto com'era.
- Durante il passaggio e il ripristino, l'assistenza vede da quanti secondi lavora il passo in corso.

## 0.1.61

- Corretto il motivo per cui, con la 0.1.60, il passaggio dello Z-Wave alla copia di Sweetplace si fermava quando
  doveva ricollegare Home Assistant alla copia: lo Z-Wave restava spento finché l'assistenza non premeva «Ripristina».

## 0.1.60

- L'assistenza di Sweetplace può portare lo Z-Wave del tuo impianto dall'add-on del suo autore alla copia che
  Sweetplace pubblica nel suo archivio, con le stesse chiavi e gli stessi dispositivi. Lo fa dalla sua console, su
  una casa alla volta, e lo Z-Wave si ferma per qualche minuto. L'add-on dell'autore resta installato e fermo, come
  copia di sicurezza, e l'assistenza può tornare indietro con «Ripristina». Se la copia non parte, Sweetlink manda
  all'assistenza le ultime righe del suo registro, al più 200.
- Per farlo Sweetlink dichiara al sistema un permesso in più (il ruolo «manager» del Supervisor): gli serve per
  installare, avviare, fermare e togliere un add-on e per fare e togliere una copia di sicurezza. Sweetlink lo usa
  solo per il passaggio dello Z-Wave e per l'azzeramento di un impianto da copiare.
- Prima di preparare un nuovo impianto da copiare, Sweetlink ferma da solo la rete di servizio dell'assistenza. Se la
  vede accesa e non riesce a fermarla, non cancella niente e lo dice.

## 0.1.59

- Se l'impianto si spegne nei primi minuti dopo l'avvio, Sweetlink non scrive più nel suo registro una riga
  sbagliata sul collegamento con l'assistenza.

## 0.1.58

- Dalla console il team può aggiornare gli altri add-on all'ultima versione del loro autore, uno alla volta,
  con una copia di sicurezza prima di ciascuno. Se un add-on non riparte o un'integrazione non torna,
  l'aggiornamento si ferma lì.

## 0.1.57

- Nell'elenco delle integrazioni che l'assistenza legge c'è anche l'indirizzo a cui ognuna è collegata,
  per esempio quello del server Z-Wave. Dell'indirizzo si invia solo l'apparecchio e la porta: password,
  chiavi, codici d'accesso e il resto dell'indirizzo restano sull'impianto e non vengono inviati.

## 0.1.56

- L'assistenza di Sweetplace può leggere dalla sua console cosa è installato sul tuo impianto: le
  applicazioni, le integrazioni e ciò che HACS ha scaricato, con le loro versioni, e gli avvisi che
  Home Assistant mostra fra le riparazioni. La lettura parte solo quando l'assistenza la chiede, e non
  cambia niente in casa. I nomi che hai dato alle integrazioni non vengono inviati. Il testo di un
  errore di un'integrazione sì, e può contenere l'indirizzo di un dispositivo della tua rete di casa.

## 0.1.55

- L'app dice all'assistenza da dove l'impianto riceve i suoi aggiornamenti: dalla versione di
  produzione di Sweetplace, dalla versione di prova, o da un'altra fonte. Dice anche quanti degli altri
  programmi installati non arrivano dal catalogo di Sweetplace. Per chi abita la casa non cambia
  niente.
- Prima di preparare un nuovo impianto da copiare, il controllo finale mostra da quale versione
  l'impianto riceve gli aggiornamenti, e l'impianto si prepara solo se è quella di produzione. Per
  confermare, la parola da scrivere nel pannello diventa PRODUZIONE.

## 0.1.54

- Nessuna novità per chi usa l'impianto: controlli in più prima che una versione nuova venga
  distribuita.

## 0.1.53

- Con Google Home collegato, l'app Google Home mostra i dispositivi scelti per i comandi vocali, con
  i loro nomi e le loro stanze, e li può accendere, spegnere e leggere. Quando un dispositivo cambia
  stato in casa, l'app Google Home lo vede da sola, senza doverla riaprire.

## 0.1.52

- Quando l'assistenza aggiorna da remoto il programma che governa la casa, l'app considera il
  programma nuovo partito bene quando il programma stesso dice di aver finito di avviarsi. Prima
  aspettava anche che uno dei suoi automatismi fosse già scattato: in una casa con pochi automatismi
  poteva non succedere affatto, e l'app rimetteva il programma di prima anche se quello nuovo
  funzionava.
- Se in quel momento l'impianto sta facendo o ripristinando una copia di sicurezza, o il suo sistema
  sta ripartendo, l'app aspetta che abbia finito prima di riaccendere il programma della casa, di
  aggiornare NetDaemon e MariaDB o di rimettere MariaDB com'era, e lo dice all'assistenza. Prima, in
  quel caso, il programma della casa poteva restare spento.
- Se MariaDB è acceso ma non ha ancora detto a Home Assistant di essere pronto, l'app non aggiorna il
  programma della casa e spiega all'assistenza cosa fare: riavviare MariaDB e riprovare.

## 0.1.51

- L'app è pronta per la versione di Home Assistant in uso negli impianti.
- Dopo l'aggiornamento di Home Assistant l'accesso da fuori casa torna a funzionare.

## 0.1.50

- Prima di installare da remoto una nuova versione del programma che governa la casa, l'app
  controlla che NetDaemon e MariaDB, i due componenti su cui il programma si appoggia, siano
  abbastanza recenti. Se non lo sono non installa niente, a meno che l'assistenza chieda di
  aggiornarli prima.
- Quando li aggiorna, spegne il programma della casa una volta sola: aggiorna prima MariaDB, poi
  NetDaemon, e lo riaccende solo quando MariaDB ha davvero finito di sistemare i suoi dati. Prima di
  aggiornare MariaDB l'app ne fa una copia di sicurezza, che resta fra le copie di sicurezza
  dell'impianto con un nome che comincia per «Sweetlink»; se l'aggiornamento di MariaDB non riesce,
  l'app rimette da sola la copia e il programma di prima, e se neanche questo riesce il programma della
  casa resta spento e l'assistenza lo sa. Di NetDaemon la copia la fa Home Assistant.
- Durante l'aggiornamento l'app dice all'assistenza a che punto è e da quanto tempo la casa è senza
  programma, e l'assistenza può interromperlo: l'app rimette le cose com'erano dove si può.
- Mentre il programma della casa si aggiorna, l'app non accetta aggiornamenti di se stessa né di
  Home Assistant; e non aggiorna il programma mentre Home Assistant o un'altra app si stanno
  aggiornando, anche se l'aggiornamento l'ha chiesto qualcuno dall'impianto. Aspetta anche che Home
  Assistant finisca le sue copie di sicurezza: prima di aggiornare qualcosa Home Assistant ne fa una, e
  se la manda a un servizio di backup esterno ci possono volere minuti, in cui il Supervisor non mostra
  ancora niente. Per saperlo l'app chiede a Home Assistant di avvisarla; se Home Assistant non lo
  permette, l'app lo scrive nel suo registro e guarda solo il Supervisor, e quei minuti restano
  scoperti.
- L'app dice all'assistenza quali versioni di NetDaemon e MariaDB sono installate e quali sono le
  ultime disponibili.

## 0.1.49

- Quando un aggiornamento chiesto dall'assistenza non va a buon fine, o l'app incontra un problema,
  l'app manda da sola all'assistenza il pezzo del suo registro che serve a capire cosa è successo:
  non serve più copiarlo a mano. Prima di mandarlo toglie chiavi e password, nelle forme che
  conosce.
- Quando serve, l'assistenza può leggere dalla sua console il registro dell'app e quello del
  programma che governa la casa; quello che legge così non viene conservato.

## 0.1.48

- Quando l'assistenza aggiorna da remoto il programma che governa la casa, mentre aspetta che il
  programma nuovo si avvii l'app manda all'assistenza, passo per passo, cosa vede. Se capisce subito
  che non sta girando il programma giusto, rimette quello di prima senza aspettare dieci minuti,
  e manda il perché.

## 0.1.47

- Quando l'assistenza aggiorna da remoto Home Assistant, l'app o il programma che governa la casa,
  l'app le dice a che punto è l'aggiornamento mentre succede, con la percentuale dello scaricamento
  quando Home Assistant la dà. Quando Home Assistant riparte lo dice subito, e poi controlla ancora
  per qualche minuto che resti acceso prima di dare l'aggiornamento per concluso.
- L'app ora chiede il programma che governa la casa nello stesso modo in cui si collega già
  all'assistenza. Dovrebbe sparire il rifiuto che sull'impianto di prova fermava l'invio da remoto.

## 0.1.46

- L'assistenza può aggiornare da remoto il programma che governa la casa. Prima di installarlo l'app
  controlla che sia proprio quello mandato; dopo, controlla che funzioni, e se non funziona rimette
  da sola quello di prima.

## 0.1.45

- Dai prossimi aggiornamenti in poi, quando l'assistenza aggiorna l'app da remoto e l'aggiornamento
  riesce, la sua console lo mostra come riuscito e non più come rifiutato. Questo aggiornamento, che
  installa la correzione, può ancora risultare rifiutato anche se è andato bene.

## 0.1.44

- Durante gli aggiornamenti l'app annota meglio nel suo registro cosa sta succedendo, così
  l'assistenza capisce più in fretta perché un aggiornamento non è partito.

## 0.1.43

- Prima di preparare un nuovo impianto, il controllo finale avvisa se Home Assistant è collegato a un
  account Home Assistant Cloud, e spiega come scollegarlo.
- Quando l'accesso dell'assistenza o dell'installatore si richiude, l'app non lascia più messaggi
  d'errore inutili nel registro di Home Assistant.

## 0.1.42

- Il pulsante del pannello per registrare l'apparecchio porta direttamente alla sua pagina di
  registrazione, anche su un computer dove si è già aperta un'altra casa.

## 0.1.41

- L'app controlla da sola le impostazioni di Home Assistant che servono all'accesso da fuori casa e
  alla protezione contro i tentativi di accesso ripetuti. Prima di correggerle mette da parte una copia
  del file che le contiene, quando il file c'è già, e di solito Home Assistant si riavvia una volta; se
  qualcosa non va, rimette tutto com'era e avvisa l'assistenza.

## 0.1.40

- Se Home Assistant blocca un indirizzo dopo troppe password sbagliate, la casa lo vede con parole
  semplici — una notifica e un avviso nel pannello — e l'assistenza potrà sbloccarlo dalla console.

## 0.1.39

- Manutenzione interna: nessuna novità per chi usa l'impianto.

## 0.1.38

- L'assistenza può aggiornare l'app Sweetlink da remoto, con una copia di sicurezza fatta prima.

## 0.1.37

- Il permesso dal pannello vale per i due account di assistenza previsti sull'impianto.

## 0.1.36

- Dal pannello decidi tu quando l'assistenza Sweetplace o l'installatore possono entrare nel tuo
  impianto. Il permesso si spegne da solo dopo dieci minuti senza attività.

## 0.1.35

Prima versione distribuita.

- Il pannello nella barra laterale mostra lo stato del collegamento con i servizi Sweetplace.
- Le persone di casa si gestiscono dal portale e compaiono nel pannello dell'apparecchio, con
  l'intestatario della casa indicato accanto al suo nome.
- L'indirizzo di casa si cambia dal portale e l'apparecchio lo aggiorna anche in Home Assistant.
- Se un cambiamento alla configurazione non va a buon fine, l'apparecchio rimette le cose com'erano
  e avvisa l'assistenza.
- L'apparecchio comunica all'assistenza quali versioni sta eseguendo, così che gli aggiornamenti
  arrivino quando servono e non a caso.
- L'assistenza può aggiornare Home Assistant da remoto, sempre con una copia di sicurezza fatta
  prima, e riportarlo alla versione precedente se serve.
