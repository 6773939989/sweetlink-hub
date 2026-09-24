# Novità

Questo è il testo che Home Assistant mostra quando propone un aggiornamento. Una voce per versione,
la più recente in cima, scritta per chi ha l'impianto in casa e non per chi lo sviluppa.

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
