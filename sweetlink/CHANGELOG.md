# Novità

Questo è il testo che Home Assistant mostra quando propone un aggiornamento. Una voce per versione,
la più recente in cima, scritta per chi ha l'impianto in casa e non per chi lo sviluppa.

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
