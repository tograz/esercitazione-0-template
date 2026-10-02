# Osservazioni — Esercitazione 0

Gruppo: C15

Componenti (nome, cognome e username GitHub di entrambi): Tommaso Graziani, tograz, Edoardo Palombi, palombi2260279

URL del repository condiviso: 

Chi ha usato la tastiera nello step 1 e nello step 2: Tommaso Graziani step 1, Edoardo Palombi step 2

Compilate insieme le osservazioni e discutete le risposte: entrambi dovete
saper spiegare le prove svolte.

## Step 1 — Hello World: compilazione ed esecuzione

Comando di compilazione: gcc -Wall -Wextra  -Wpedantic hello.c -o hello

Comando di esecuzione e risultato osservato: ./hello > output.txt
prima di inserire "> output.txt" il testo inserito tra virgolette veniva stampato nel terminale, dopo l'aggiunta l'output è distinto dal resto in quanto inserito direttamente nel file .txt.

Che cosa ho capito su sorgente ed eseguibile: Il file sorgente è modificabile direttamente in emacs ed è ciò che viene compilato per poi produrre un eseguibile, l'applicazione per l'appunto eseguita in locale, più pesante a livello di memoria su disco.

Output richiesto e comportamento del programma prima della modifica: Hello, computational physics! prima della modifica il programma hello non stampava nulla quando eseguito, solo dopo aver ricompilato hello.c con il comando make printa l'output desiderato. 

Esito dopo la modifica e spiegazione della correzione: dopo la modifica il programma stampa l'output desiderato.

## Step 1 — Git

Quali file ho incluso nel commit e perché: hello.c e osservazioni.md perché sono i file su cui è stato necessario effettuare modifiche in locale da inviare poi con push. 

Come ho verificato che la versione provata sia presente su GitHub: Ho aperto il repository su github dopo git push e verificato che il messaggio dell'ultimo commit corrispondesse a quellogiusto, abbiamo anche controllato i file.

Scrivo questa frase come prova prima di fare git pull modificando direttamente dal repository su github.

Che cosa ho osservato prima e dopo `git pull`, e perché non serve un nuovo clone: prima di git pull il comando git log --oneline -5 non mostrava il messaggio dell'ultimo commit effettuato direttamente dal repository online, mentre dopo pull le modifiche sono state importate e anche il messaggio del commit risulta visibile. osservazioni.md risulta modificato e la frase di prova scritta sopra è visibile in locale.

## Step 2 — Eco: prima prova

Argomenti passati, comando e risultato: ciao 12 3.5, ./eco ciao 12 3.5, ciao 12 3.500000 dentro eco.txt

Che cosa posso concludere: il programma restituisce l'output desiderato con decimali giusti

## Step 2 — Eco: seconda prova

Argomenti passati, comando e risultato: ciao dodici 3.5, ./eco ciao dodici 3.5, ciao 0 3.50000 

Che cosa ho capito su testo, conversioni e stampa: atoi ha comunque restituito un intero ma è 0 non avendo trovato cifre numeriche.

## Step 2 — Risultato ed errori

Previsioni per l'esecuzione con argomenti validi e per quella con `dodici`:con dodici era previsto un errore mentre il file gira normalmente restituendo 0 come intero.

Contenuto di `eco.txt`, messaggi nel terminale e codici di uscita osservati: nel primo caso l'output è corretto, con dodici appare 0 e i codici di uscita osservati con echo &? sono sempre 0

Come un controllo automatico può riconoscere un errore: si può aggiungere per argv[2] e argv[3] un controllo carattere per carattere, in un ciclo iterativo per esempio, con una funzione che mostri se si tratta di una cifra o di un carattere non convertibile da atoi e atof.

## Step 2 — Parametri e calcolo fisico

Quando serve ricompilare e quando basta cambiare gli argomenti: serve ricompilare se viene modificato qualche valore scritto nel sorgente, mentre inserendo solo nuovi argomenti nel terminale il file non richiede modifiche e produce output diversi.

## Step 2 — Git

Come riconosco nella cronologia i commit dei due step: dai messaggi inseriti in git commit -m "messaggio" direttamente visibili.

Come ho verificato che la versione finale sia presente su GitHub: controllando online direttamente nel repository i file e che i messaggi dell'ultimo commit sul terminale e sul sito coincidessero.
