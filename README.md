# Progetto Algoritmi Paralleli Sistemi Distribuiti
Si realizzi una piattaforma per l’esecuzione parallela di modelli ad automi cellulari. Si considerino solo celle il cui valore può essere un intero (int) pari a ‘0’ o a ‘1’. 

In particolar modo un modello ad automa cellulare sarà definito dalla funzione: voidtransitionFunction(int x, int y) che definisce la funzione di transizione per la generica cella (x,y).

La piattaforma dovrà eseguire tale modello ad automa cellulare in parallelo considerando un sistema misto a memoria condivisa e distribuita, ovvero utilizzando MPIe i thread Posix, e partizionando il dominio dell’automa sia sull’ascissa che sull’ordinata. L’andamento dell’esecuzione deve essere visualizzato istante per istante in un visualizzatore realizzato con la libreria ‘Allegro’. 

Il modello (che sarà fornito in input alla piattaforma durante l’esame) consiste nella implementazione della   sopracitata   funzione transitionFunction nella quale verranno lette e scritte le matrici di lettura e scrittura che dovranno chiamarsi obbligatoriamente readM e writeM e realizzate come un array monodimensionale al quale si accede con l’ausilio di una macro, ‘v’, ovvero ad esempio nel seguente modo: writeM[v(x+1,y)]=readM[v(x,y)]. Oltre a questo, un modello ha anche un file di configurazione (Configuration.txt) e un file di input (Input.txt). Il file di configurazione contiene i seguenti valori interi (uno per riga):
- Numero di partizioni lungo la X.
- Numero di partizioni lungo la Y.
- Numero di thread per processo MPI.
- Numero di step.

Mentre il file di input conterrà lo stato iniziale del dominio, come ad esempio:

00000000000000000000

00000000001000000000 

00000000000100000000 

00000000011100000000 

00000000000000000000 

00000000000000000000 

00000000000000000000 

00000000000000000000 

La descrizione del progetto è disponibile qua: [Presentazione Progetto Algoritmi Paralleli e Sistemi Distribuiti](https://github.com/matte18it/ProgettoAPSD/blob/main/ProgettoAPSD.pdf)

# 📼 Demo Video 📼
<div align="center">
  <img src="https://github.com/matte18it/ProgettoAPSD/blob/main/Demo.gif" alt="Palkia">
</div>

# ❗️DISCLAIMER❗️
Alla realizzazione del progetto hanno contribuito gli studenti dell'Università della Calabaria:
<ul>
  <li>Matteo Canino</li>
  <li>Pierfrancesco Napoli</li>
</ul>
