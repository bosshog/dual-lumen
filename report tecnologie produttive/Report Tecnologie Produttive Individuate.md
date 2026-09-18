# Report Tecnologie Produttive Individuate — Cannula Dual Lumen

> Bozza in Markdown. Lo stile grafico (copertina, indice, immagini con didascalie, footer
> aziendale) verrà applicato in un secondo momento, allineandolo al
> [Report Reverse Engineering Avalon Elite 19Fr](../report%20reverse%20engineering/Report%20Reverse%20Engineering%20Avalon%20Elite%2019Fr.pdf).

## Executive Summary

Per la realizzazione del prototipo di cannula dual lumen per ECLS ci si è concentrati sulla
tecnologia del dipping, sfruttando l'esperienza pregressa maturata su cannule monolume. La
sfida principale è risultata l'adattamento del processo di estrazione dei mandrini — già
validato per le cannule monolume — alla geometria specifica dei mandrini dual lumen. Sono
stati condotti quattro tentativi successivi, che hanno portato a un processo funzionante per
l'estrazione dei mandrini e alla produzione di un campione conforme dal punto di vista del
setto, pur con una sezione della porzione dual lumen ancora fuori specifica. A seguito di
questi risultati, è stata confermata la scelta del dipping rispetto all'estrusione, ed è stata
individuata la necessità di rivedere il design dei mandrini prototipo.

## 1. Scopo

- Individuare le tecnologie produttive per la realizzazione del prototipo di cannula dual
  lumen per ECLS.
- Risolvere le criticità specifiche introdotte dalla geometria dual lumen rispetto alle
  cannule monolume già realizzate in passato.
- Confermare la tecnologia di riferimento (dipping vs estrusione) e definire i prossimi passi
  di sviluppo.

## 2. Descrizione generale

Il progetto ha per oggetto la realizzazione di un prototipo di cannula dual lumen per ECLS,
size 19 Fr — lo stesso size oggetto del report di reverse engineering: un dispositivo dotato
di due lumi interni, uno dedicato all'aspirazione e uno alla reinfusione, ciascuno collegato a
un proprio raccordo esterno.

Il prototipo non è dual lumen su tutta la lunghezza: prevede una porzione a singolo lume in
prossimità della punta, dove è presente il solo lume di aspirazione. Il lume di reinfusione si
interrompe infatti prima, in corrispondenza della reinfusion port, posizionata a circa 6 cm
dalla punta. Risalendo verso i raccordi, i due lumi corrono affiancati fino a dividersi, poco
prima dei connettori, in due condotti separati che confluiscono ciascuno nel proprio raccordo.

Il progetto si affianca a un'attività di reverse engineering della cannula competitor Avalon
Elite 19Fr, già completata, che ha fornito un riferimento dimensionale e costruttivo per la
definizione del prototipo.

## 3. Tecnologie produttive individuate

### 3.1. Scelta tecnologica: dipping vs estrusione

Ci si è concentrati sulla tecnologia del dipping, in contrapposizione all'estrusione, per
sfruttare l'esperienza pregressa maturata negli anni, come riportato nel contratto di
progetto. In parallelo, è stato comunque
richiesto a un fornitore esterno un prototipo per estrusione di un tubo bilume in
poliuretano.

A seguito dei risultati del Tentativo 4 (§4.6), è stata confermata la scelta del dipping per
ottenere la porzione dual lumen della cannula, senza passare all'estrusione.

### 3.2. Processo di dipping — panoramica generale

Per ottenere la cannula dual lumen per dipping:

1. Due mandrini (uno per il lume di aspirazione, uno per il lume di reinfusione), accoppiati
   in qualche modo.
2. Immersioni ripetute in soluzione di poliuretano + THF, per ottenere uno strato base di
   poliuretano sui mandrini.
3. Deposizione di 3 segmenti di coil e di 3 basket in acciaio sopra lo strato base, per la
   resistenza meccanica.
4. Strato esterno di poliuretano, per dipping o per laminazione.
5. Rimozione dei mandrini.

### 3.3. Problema principale del dipping

Il problema principale del dipping — non specifico alla cannula dual lumen, ma generale a
tutte le cannule prodotte con questa tecnologia — è l'estrazione dei mandrini una volta
evaporato il THF.

## 4. Estrazione mandrini: sviluppo e tentativi

### 4.1. Soluzione validata su cannule monolume

Per le cannule monolume già realizzate in passato, si stira un tubo in PTFE sul mandrino,
applicando una temperatura di circa 400°C e una trazione di 5 kg. Il PTFE resta in posizione
grazie agli aggrappaggi presenti sul mandrino: senza questi aggrappaggi, una volta rimosso il
peso della trazione, il PTFE si ritirerebbe. Il mandrino con il PTFE così applicato attraversa
le varie fasi del processo di realizzazione della cannula (dipping, posizionamento segmenti
coil e basket) e viene infine intestato in cima e in fondo, operazione che permette il
distacco del PTFE dal mandrino e la successiva rimozione del tubo PTFE.

Si riesce a sfilare il mandrino perché il PTFE non si attacca all'acciaio del mandrino,
mentre il poliuretano si aggrapperebbe tenacemente all'acciaio, rendendo l'estrazione diretta
impossibile senza l'interposizione del PTFE. Il passaggio finale — estrazione del PTFE
dall'interno del tubo in poliuretano — è una manovra abbastanza agevole: si afferra il PTFE
con una pinza e lo si torce/tira fino al completo distacco.

### 4.2. Geometria dei mandrini dual lumen — la sfida specifica

Il mandrino aspirazione presenta una cava (concavità marcata) che alloggia il mandrino di
reinfusione. Il processo di stiratura del tubo PTFE, validato sui mandrini monolume, non
riesce a far aderire il PTFE nella parte concava del mandrino di aspirazione.

### 4.3. Tentativo 1 — Teflonatura permanente (fornitore esterno)

È stato valutato un processo di teflonatura permanente sui mandrini, affidato a un fornitore
esterno. Il processo di applicazione del coating
permanente ha generato una superficie rugosa al tatto, presumibilmente non ottimale per il
distacco della cannula finita.

Un utile riferimento di confronto viene da due mandrini campione con PTFE permanente (uno
verde, uno nero) forniti in passato dal cliente e usati per realizzare due cannule monolume.
In entrambi i casi l'estrazione è stata possibile solo realizzando lo strato esterno tramite
dipping, senza laminazione: quando è stata usata la laminazione, non è stato possibile
estrarre la cannula. Il mandrino verde presenta inoltre un certo grado di rugosità
superficiale al tatto: l'estrazione è risultata agevole, ma poiché la superficie interna della
cannula copia quella del mandrino, la rugosità ha fatto perdere la trasparenza del
poliuretano, rendendo la cannula opaca. Il mandrino nero, con superficie molto più liscia,
dovrebbe evitare il problema dell'opacità, ma non è stato possibile rimuoverlo se non dopo
una settimana.

Nonostante la finitura non ottimale, i mandrini teflonati sono stati comunque utilizzati per
realizzare una prima cannula dual lumen completa, utilizzando il coil di una cannula 19 Fr.
Per lo strato esterno è stato adottato il
dipping "over coil" (anziché la laminazione usata per la 19 Fr), scelta ritenuta accettabile
anche alla luce di quanto osservato sui mandrini campione. L'esito è stato negativo: non è
stato possibile estrarre i mandrini, e per rimuoverli è stato necessario sciogliere la
cannula nel THF, sacrificando il prototipo.

### 4.4. Tentativo 2 — PTFE spray

A seguito del fallimento del Tentativo 1, è stata valutata l'applicazione di PTFE spray sui
mandrini. Un test preliminare su geometria semplice (spina di acciaio cilindrica, diametro
6 mm → PTFE spray → dipping substrato → coil 19 Fr → dipping strato esterno) ha dato esito
positivo: il giorno dopo la spina si è sfilata agevolmente.

Il PTFE spray è stato quindi applicato sopra i mandrini già teflonati permanentemente
(superficie rugosa), realizzando una cannula dual lumen completa. L'esito è stato negativo:
dopo la maturazione del PU, l'estrazione non è stata comunque possibile. I mandrini sono
stati rimossi tagliando PU e coil (senza sciogliere nel THF, per poter ispezionare i residui).
La superficie interna della cannula è risultata piena di residui di PTFE; oltre al PTFE
depositato con lo spray, sono stati trovati anche pezzi del coating permanente applicato dal
fornitore esterno nel Tentativo 1 — ulteriore riprova della non adeguatezza di quel
trattamento. I residui non sono accettabili per questa cannula.

Resta aperto il punto sul perché il risultato positivo ottenuto sul pin semplice non si sia
riprodotto sui mandrini dual lumen reali — da capire se dovuto alla rugosità pregressa, alla
geometria complessa, o altro.

### 4.5. Tentativo 3 — Ritorno al tubo PTFE stirato (soluzione adottata)

Indipendentemente dalla causa del fallimento del Tentativo 2, si è tornati al tubo in PTFE
stirato per entrambi i mandrini. Data la geometria (concavità sul mandrino aspirazione, curve
sul mandrino reinfusione), non è stato possibile applicare il processo di stiratura usato per
la 19 Fr con i parametri standard. La soluzione adottata è stata l'uso di una temperatura
molto più alta, oltre 600°C, raggiunta con un phon industriale (strumento non usato
abitualmente perché meno preciso rispetto alla hot box Beahm, modello Balloon Development
System 210-A, normalmente usata per precisione e ripetibilità).

Sul mandrino reinfusione il PTFE ha aderito abbastanza agevolmente, con una trazione molto
leggera applicata che riduce notevolmente il ritiro del PTFE una volta raffreddato. Come
contropartita, con trazione così leggera il tubo PTFE mantiene delle grinze anche a contatto
con il mandrino, che si ritrovano poi nel prototipo di cannula come segni sulla superficie
interna. Sul mandrino aspirazione il PTFE ha formato inizialmente una membrana tesa sulla
parte concava, lavorata manualmente (a caldo e a freddo) spingendola dentro la cava, con
esito positivo: la membrana si è deformata a sufficienza per aderire anche nella zona
concava. Su entrambi i mandrini, la quasi assenza di ritiro del PTFE dopo l'intestatura
(grazie alla trazione molto leggera) consente di evitare di dover prevedere aggrappaggi sul
mandrino, a differenza di quanto necessario con la trazione di 5 kg usata sui mandrini
monolume.

**Processo di dipping stratificato (formazione del setto)**

1. Dipping del mandrino reinfusione da solo, per ottenere un primo strato base.
2. Accoppiamento del mandrino reinfusione (con il suo primo strato base) al mandrino
   aspirazione, tramite un anello di PU ottenuto tagliando una piccola porzione di guaina
   della 19 Fr (la stessa guaina normalmente usata nel processo di laminazione), per tenere
   adesi i due mandrini.
3. Dipping di entrambi i mandrini insieme, per ottenere lo strato base della cannula finale.
4. Il mandrino reinfusione risulta così con un doppio strato base (spessore maggiore).
5. Il primo strato base del mandrino reinfusione, nella zona tra i due mandrini, funge da
   setto della porzione dual lumen della cannula finale.

L'anello di PU produce però un rigonfiamento nel corpo della cannula, nel punto di
accoppiamento, che impedisce l'uso del coil 19 Fr preformato: le spire del coil, già formate,
non riescono a superare il rigonfiamento facendole scorrere lungo il mandrino. La soluzione
adottata è stata ottenere il coil partendo da una piattella in acciaio, avvolta direttamente
lungo il corpo della cannula anziché preformata, superando così il vincolo.

Resta un punto aperto per sviluppi futuri: il fatto di aver dippato solo il mandrino
reinfusione prima dell'accoppiamento potrebbe essere rivisto — potrebbe essere necessario
dippare anche il mandrino aspirazione prima di accoppiarlo.

Con questo processo è stata realizzata una prima cannula dual lumen completa: l'estrazione
dei mandrini è riuscita, risolvendo il problema critico di estrazione. L'analisi della
cannula ha però rilevato una lacerazione del setto tra i due mandrini, nel punto dove questi
si dividono (vicino alla zona dei connettori), che mette in comunicazione i due lumi — difetto
critico, non accettabile. Si ipotizza che la rottura sia dovuta a uno scarso accoppiamento dei
due mandrini in quella zona, riconducibile a un difetto del mandrino aspirazione non
riconosciuto in fase di design.

### 4.6. Tentativo 4 — Tubo termoretraibile + inserto, verso il coil 19 Fr preformato

Per i prossimi campioni si vuole tornare a usare il coil 19 Fr preformato, anziché il coil da
piattella avvolta manualmente. Questo non è compatibile con l'anello di PU usato nel
Tentativo 3 per l'accoppiamento dei mandrini, a causa del rigonfiamento che impedisce il
passaggio delle spire già preformate.

A seguito della lacerazione del setto riscontrata sulla cannula del Tentativo 3, il difetto è
stato individuato alla fine della cava del mandrino aspirazione (nella zona di separazione
dei due mandrini): in quel punto era stato erroneamente creato uno spazio eccessivo. È stato
quindi introdotto un inserto per riempire tale spazio in eccesso, correzione resa possibile
dal fatto che il tubo PTFE ricopre il mandrino insieme all'inserto. Anche questo aspetto
verrà corretto a monte con il nuovo design dei mandrini.

Per l'accoppiamento dei mandrini, è stato adottato un approccio intermedio con un tubo
termoretraibile al posto dell'anello di PU:

1. Il tubo termoretraibile è stato applicato sulla parte terminale del mandrino reinfusione,
   in corrispondenza della porta di reinfusione della cannula (circa 6 cm dalla punta) —
   punto dove il mandrino reinfusione termina. Questo punto è distinto dalla zona di
   divisione dei due mandrini, che si trova più in zona prossimale, prima che i due lumi/tubi
   diventino manicotti/raccordi.
2. È stata dippata inizialmente solo la parte prossimale (lato manicotti/raccordi),
   fermandosi appena dopo la zona di divisione dei due mandrini.
3. L'obiettivo era che la struttura in PU così ottenuta sulla parte prossimale mantenesse i
   due mandrini in posizione accoppiata anche dopo la successiva rimozione del tubo
   termoretraibile.
4. Solo dopo la rimozione del termoretraibile si è proceduto a dippare la parte distale dei
   mandrini (punta della cannula), con l'obiettivo di poter usare il coil 19 Fr preformato
   senza più l'ostacolo del rigonfiamento.

La reinfusion port è stata realizzata su questo campione rimuovendo lo strato di PU in
corrispondenza della fine del mandrino reinfusione.

**Esito**

- **Estrazione dei mandrini**: agevole. Il PTFE ha aderito meglio ai mandrini grazie a una
  leggera ottimizzazione del processo di stiramento/riscaldamento del tubo PTFE — il processo
  resta comunque da ottimizzare ulteriormente.
- **Accoppiamento mandrini**: una volta rimosso il tubo termoretraibile, i due mandrini si
  sono leggermente disaccoppiati nel punto dove finisce il mandrino di reinfusione, con un
  conseguente aumento del diametro esterno in quel punto. Anche in questo caso l'aumento di
  diametro ha impedito l'uso del coil 19 Fr preformato: è stato quindi necessario, ancora una
  volta, ottenere il coil da una piattella in acciaio avvolta direttamente lungo il corpo
  della cannula, anziché preformata.
- **Setto**: il campione non presenta fori nel setto — conforme, nessuna comunicazione tra i
  due lumi.
- **Sezione della porzione dual lumen**: fuori specifica, perché il PTFE sul mandrino
  aspirazione spinge il mandrino reinfusione verso l'esterno.

## 5. Decisioni e prossimi passi

- È stata confermata la scelta del dipping per ottenere la porzione dual lumen della cannula,
  senza passare all'estrusione (vedi §3.1).
- Il design dei mandrini va rivisto, per migliorare l'accoppiamento tra mandrino aspirazione
  e mandrino reinfusione e per tenere in considerazione la presenza del tubo in PTFE, che
  aumenta il diametro dei mandrini.
- Insieme al cliente è stato deciso di proseguire con il tubo in PTFE stirato come soluzione
  per l'estrazione dei mandrini, sospendendo per il momento i test sui mandrini con PTFE
  permanente (teflonatura permanente, Tentativo 1).

## 6. Conclusioni

Il processo di dipping, unito al tubo in PTFE stirato per l'estrazione dei mandrini, si è
dimostrato in grado di produrre un campione di cannula dual lumen con setto conforme (nessuna
comunicazione tra i lumi). Restano da risolvere due criticità aperte prima di poter
considerare il processo maturo: la sezione della porzione dual lumen fuori specifica, causata
dall'interazione tra il tubo PTFE e il mandrino aspirazione, e l'impossibilità — in tutti i
tentativi condotti finora — di utilizzare il coil 19 Fr preformato al posto della piattella
avvolta manualmente. Entrambi i punti sono legati al design attuale dei mandrini, la cui
revisione è stata individuata come prossimo passo necessario.

## Collegamenti

- Progetto trasversale **PTFE-spray** (vedi [LINKS.md](../LINKS.md)) — approfondimenti sul
  confronto tra spray PTFE medical-grade come release agent.
- Note grezze di raccolta informazioni, base di questo report:
  [note-raccolta-informazioni.md](note-raccolta-informazioni.md).
- Report di reverse engineering della cannula competitor Avalon Elite 19Fr:
  `report reverse engineering/`.
