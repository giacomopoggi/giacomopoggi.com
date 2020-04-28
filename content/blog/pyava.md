+++
date = "2020-04-22"
title = "Pyava: un semplice launcher per emulatori scritto in Python"
+++

Pyava è un semplice launcher per emulatori che ho scritto nell'ottobre del 2017 in Python (per la precisione Python 3), il linguaggio di programmazione che studiavo in quel momento.  
Si configura come un comodo menù portatile per avviare i propri giochi.  
L'idea è stata ispirata da [Yava](https://github.com/Beluki/Yava), un programma molto simile scritto in linguaggio C# (ed il nome Pyava stesso rappresenta una crasi delle parole **P**ython e **Yava**).  
Pyava può essere scaricato gratuitamente da [GitHub](https://github.com/giacomopoggi/Pyava).

![alt text](/images/pyava-screenshot.png)
*Pyava su Windows 10*

**Tasti rapidi**

| Tasto  | Funzione                                                       |
| ------ | -------------------------------------------------------------- |
| Esc    | Chiude il programma.                                           |
| Tab    | Sposta la selezione dal pannello sinistro al destro.           |
| Ctrl+A | Mostra un messaggio informativo.                               |
| Ctrl+R | Ricarica il file config.ini senza chiudere il programma.       |
| Ctrl+S | Imposta un separatore personalizzato per dividere i parametri. |

**Configurazione**

Pyava deve essere configurato utilizzando un file denominato "config.ini". Questo file contiene tutto ciò che Pyava ha bisogno di sapere sulle cartelle ed i file che dovrà gestire.

Questo esempio di configurazione è stato utilizzato nella generazione dello screeenshot precedente:
```ini
[Game Boy]
games = C:\Games\Game Boy\
executable = C:\Emulators\BGB\bgb.exe
extensions = .zip, .gb

[Nintendo Entertainment System]
games = C:\Games\Nintendo Entertainment System\
executable = C:\Emulators\Mesen\Mesen.exe
extensions = .7z
parameters = /fullscreen, /DoNotSaveSettings
```
I parametri e le estensioni sono separati dal carattere ",". Si può impostare un separatore personalizzato utilizzando l'apposito tasto rapido, ma il separatore è reimpostato sul carattere "," ogni volta che viene selezionata una piattaforma diversa dalla lista.