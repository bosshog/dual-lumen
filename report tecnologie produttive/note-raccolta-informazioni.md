# Note raccolta informazioni — Report di tecnologie produttive individuate

> Materiale grezzo raccolto in conversazione, da usare come base per la stesura del report finale
> "Report di tecnologie produttive individuate". Non ancora rielaborato in forma di report.

## Contesto progetto

- Progetto per la realizzazione di un prototipo di **cannula dual lumen per ECLS**.
- La cannula non è bilume su tutta la lunghezza: comprende una porzione a **singolo lume** vicino
  alla punta. Il **lume di reinfusione termina in corrispondenza della reinfusion port, a circa
  6 cm dalla punta**. I due lumi confluiscono in
  **due raccordi separati**.

## Attività 1 — Reverse engineering (completata)

- Analisi della cannula dual lumen competitor **Avalon Elite 19 Fr**
  (https://www.getinge.com/it/prodotti/catetere-avalon-elite).
- Report già prodotto, si trova in `report reverse engineering/`.

## Attività 2 — Tecnologie produttive individuate (oggetto di questo report)

Le tecnologie individuate riguardano **tutta la cannula**, non solo il tratto bilume.

### Scelta tecnologica: dipping vs estrusione

- Ci si è concentrati sulla tecnologia del **dipping**, in contrapposizione all'**estrusione**,
  per sfruttare l'esperienza pregressa maturata negli anni.
- Anche nel **contratto** è riportato che si vuole **prediligere il dipping** rispetto ad altre
  tecnologie.
- In parallelo, è stato richiesto anche un **prototipo per estrusione** di un tubo bilume in
  poliuretano tramite **fornitore esterno**, dato che l'estrusione richiede macchinari dedicati
  non disponibili internamente.

### Processo di dipping — panoramica generale

Per ottenere la cannula dual lumen per dipping:

1. Due **mandrini** (uno per il lume di aspirazione, uno per il lume di reinfusione), accoppiati
   in qualche modo.
2. **Immersioni ripetute** in soluzione di **poliuretano + THF** → strato base di poliuretano sui
   mandrini.
3. Deposizione di **3 segmenti di coil** e di **3 basket** in acciaio sopra lo strato base, per
   la resistenza meccanica.
4. **Strato esterno** di poliuretano, per dipping o per laminazione.
5. **Rimozione dei mandrini**.

### Problema principale del dipping

Il problema principale del dipping (non specifico alla cannula dual lumen, ma generale a tutte le
cannule prodotte con questa tecnologia) è l'**estrazione dei mandrini** una volta evaporato il THF.

## Estrazione mandrini — soluzione validata su cannule monolume

Per le cannule monolume già realizzate in passato:

- Si stira un **tubo in PTFE** sul mandrino, applicando una **temperatura di circa 400°C** e una
  **trazione di 5 kg**. Il PTFE resta in posizione grazie agli **aggrappaggi** presenti sul
  mandrino: senza questi aggrappaggi, una volta rimosso il peso della trazione, il PTFE si
  ritirerebbe.
- Il mandrino con il PTFE così applicato attraversa le varie fasi del processo di
  realizzazione della cannula (**dipping**, posizionamento segmenti **coil** e **basket**) e
  viene infine **intestato** in cima e in fondo, operazione che permette il **distacco del
  PTFE dal mandrino** e la successiva rimozione del tubo PTFE.
- Si riesce a sfilare il mandrino perché **il PTFE non si attacca all'acciaio** del mandrino,
  mentre il **poliuretano si aggrapperebbe tenacemente all'acciaio**, rendendo l'estrazione
  diretta **impossibile** senza l'interposizione del PTFE.
- **Passaggio finale**: estrazione del PTFE dall'interno del tubo in poliuretano — manovra
  abbastanza agevole. Si afferra il PTFE con una pinza e si **torce/tira** fino al completo
  distacco dal tubo in poliuretano ottenuto.

## Geometria dei mandrini dual lumen — la sfida specifica

- Il **mandrino aspirazione** presenta una **cava** (concavità marcata) che alloggia il mandrino
  di reinfusione.
- Il processo di **stiratura del tubo PTFE** (validato sui mandrini monolume) **non riesce a far
  aderire il PTFE nella parte concava** del mandrino di aspirazione.

## Tentativo 1 — Teflonatura permanente (fornitore esterno)

- Valutato un processo di **teflonatura permanente** sui mandrini, affidato a un fornitore
  esterno (competenza non disponibile internamente).
- Il fornitore ha **sabbiato** i mandrini prima del rivestimento PTFE, alterando la **finitura
  superficiale** — parametro critico per il progetto, segnalato come tale fin dall'accordo
  iniziale.
- Il fornitore aveva concordato di usare **trattamento al plasma** invece della sabbiatura, ma ha
  poi deciso **unilateralmente e senza comunicazione preventiva** di procedere comunque con la
  sabbiatura.
- L'alterazione della finitura è visibile sulle porzioni di mandrino non coperte da PTFE.
- Introduce una **variabile non prevista** nel processo di sviluppo: non è possibile stabilire
  a priori se/quanto influirà sul risultato finale; se emergono problemi, non sarà più possibile
  distinguere l'effetto del PTFE da quello della sabbiatura pregressa.
- Investimento significativo di tempo/risorse nella realizzazione dei mandrini prototipo
  coinvolti.
- Il **fornitore ha confermato** di aver sabbiato i mandrini.
- **Esito qualità**: finitura superficiale **non ottimale** — al tatto si percepiscono
  **rugosità**, mentre la superficie dovrebbe essere **liscia** per facilitare il distacco del
  poliuretano dal mandrino.
- Confronto: in passato il **cliente** aveva fornito due mandrini campione con PTFE permanente
  (uno **verde**, uno **nero**). Usati per realizzare due cannule monolume:
  - **Mandrino verde**: presenta un certo grado di **rugosità superficiale**, percepibile al
    tatto. **Estrazione agevole**. Poiché la superficie interna della cannula copia la superficie
    del mandrino, la rugosità fa **perdere la trasparenza del poliuretano**: la cannula risulta
    **opaca**.
  - **Mandrino nero**: superficie **molto più liscia**, che dovrebbe quindi evitare il problema
    dell'opacità. **Non è stato possibile rimuovere il mandrino se non dopo una settimana**.
  - In entrambi i casi, l'estrazione è stata possibile solo realizzando lo strato esterno
    tramite **dipping**, senza laminazione: quando è stata usata la **laminazione** per lo
    strato esterno, **non è stato possibile estrarre la cannula**. L'impossibilità di usare il
    processo di laminazione con questi mandrini è un **fattore aggiuntivo** che sconsiglia
    l'adozione della teflonatura permanente.
  - Aspetto da valutare in caso si decidesse di proseguire i test sul coating permanente: il
    compromesso tra trasparenza (superficie liscia) e facilità di estrazione (superficie rugosa)
    emerso dal confronto tra i due mandrini campione.

### Prima cannula dual lumen realizzata (con mandrini teflonati permanenti)

- Nonostante la finitura non ottimale, i mandrini sono stati comunque usati per realizzare una
  cannula dual lumen completa.
- Usato il **coil di una cannula 19 Fr**, fornito dal cliente nell'ambito di un progetto
  precedente (cannula monolume 19 Fr) — riutilizzabile perché la size coincide (19 Fr).
- Per lo strato esterno: **dipping "over coil"** (mentre per la 19 Fr si era usata la
  **laminazione**). L'adozione del dipping over coil è comunque ritenuta accettabile.
- **Esito**: **non è stato possibile estrarre i mandrini**. Per rimuoverli è stato necessario
  **sciogliere la cannula nel THF** — prototipo sacrificato.

## Tentativo 2 — PTFE spray

- A seguito del fallimento, valutata l'applicazione di **PTFE spray** sui mandrini.
- **Test preliminare** su geometria semplice: spina di acciaio cilindrica, diametro 6mm →
  PTFE spray → dipping substrato → coil 19 Fr → dipping strato esterno.
  **Esito positivo**: il giorno dopo la spina si è sfilata agevolmente.
- **Applicazione su mandrini reali**: PTFE spray applicato **sopra** i mandrini già teflonati
  permanentemente (superficie rugosa), realizzata una cannula dual lumen completa.
  **Esito negativo**: dopo la maturazione del PU, l'estrazione **non è stata comunque possibile**.
  Rimossi i mandrini tagliando PU e coil (non sciolto nel THF, per poter ispezionare i residui).
  **Riscontro**: superficie interna della cannula **piena di residui di PTFE**. Oltre al PTFE
  depositato con lo spray, trovati anche **pezzi del coating permanente** applicato dal fornitore
  esterno (Tentativo 1) — ulteriore riprova della **non adeguatezza di quel trattamento**.
  Residui non accettabili per questa cannula.
  - Punto aperto: il risultato positivo sul pin semplice non si è riprodotto sui mandrini dual
    lumen reali — da capire se dovuto alla rugosità pregressa, alla geometria complessa, o altro.

## Tentativo 3 — Ritorno al tubo PTFE stirato (soluzione adottata)

- Indipendentemente dalla causa del fallimento precedente, si è tornati al **tubo in PTFE
  stirato** per entrambi i mandrini.
- Problema: data la geometria (concavità sul mandrino aspirazione, curve sul mandrino
  reinfusione), non è stato possibile applicare il processo di stiratura usato per la 19 Fr con
  i parametri standard.
- **Soluzione**: temperatura molto più alta, **oltre 600°C**, raggiunta con un **phon
  industriale** (strumento non usato abitualmente perché meno preciso rispetto alla **hot box
  Beahm, modello Balloon Development System 210-A**,
  https://beahmdesigns.com/mfg-equipment/balloon-development-system-model-210-a/, normalmente
  usata per precisione e ripetibilità).
- **Mandrino reinfusione**: PTFE aderito abbastanza agevolmente. Applicata una **trazione molto
  leggera**, che riduce notevolmente il ritiro del PTFE una volta raffreddato (nota positiva).
  **Contropartita**: con trazione così leggera il tubo PTFE mantiene delle **grinze** anche a
  contatto con il mandrino; queste grinze si ritrovano poi nel prototipo di cannula come **segni
  sulla superficie interna**.
- **Mandrino aspirazione**: il PTFE ha formato inizialmente una **membrana tesa** sulla parte
  concava. Lavorata manualmente (a caldo e a freddo), spingendola dentro la cava.
  **Esito positivo**: la membrana si è deformata a sufficienza per aderire anche nella zona
  concava.
- **Su entrambi i mandrini**, la quasi assenza di ritiro del PTFE dopo l'intestatura (grazie alla
  trazione molto leggera) consente di **evitare di dover prevedere aggrappaggi sul mandrino**
  (a differenza di quanto necessario con la trazione di 5 kg usata sui mandrini monolume).

### Processo di dipping stratificato (formazione del setto)

1. **Dipping del mandrino reinfusione da solo** → primo strato base.
2. **Accoppiamento** del mandrino reinfusione (con il suo primo strato base) al mandrino
   aspirazione, tramite un **anello di PU** ottenuto tagliando una piccola porzione di **guaina
   della 19 Fr** (la stessa guaina normalmente usata nel processo di **laminazione**), in modo da
   tenere adesi i due mandrini.
3. **Dipping di entrambi i mandrini insieme** → strato base della cannula finale.
4. Risultato: il mandrino reinfusione ha un **doppio strato base** (spessore maggiore).
5. Il **primo strato base del mandrino reinfusione**, nella zona tra i due mandrini, **funge da
   setto** della porzione bilume della cannula finale.

**Effetto collaterale dell'anello di PU**: produce un **rigonfiamento** nel corpo della cannula,
nel punto di accoppiamento. Tale rigonfiamento **impedisce l'uso del coil 19 Fr preformato**,
perché le spire del coil (già formate) non riescono a superare il rigonfiamento facendole
scorrere lungo il mandrino. **Soluzione adottata**: il coil è stato ottenuto partendo da una
**piattella in acciaio**, avvolta **direttamente lungo il corpo della cannula** (anziché
preformata), superando così il vincolo del rigonfiamento.

> Punto aperto per sviluppi futuri: il fatto di aver dippato solo il mandrino reinfusione prima
> dell'accoppiamento potrebbe essere rivisto — forse sarà necessario dippare anche il mandrino
> aspirazione prima di accoppiarlo.

### Prima cannula dual lumen completa con questo processo

- **Estrazione dei mandrini riuscita** — problema critico di estrazione risolto.
- **Analisi della cannula**: rilevata una **lacerazione del setto** tra i due mandrini, nel punto
  dove questi si dividono (vicino alla zona dei connettori). La lacerazione **mette in
  comunicazione i due lumi** — **difetto critico, non accettabile**.
- **Ipotesi di causa**: rottura forse dovuta a uno **scarso accoppiamento** dei due mandrini in
  quella zona, riconducibile a un **difetto del mandrino aspirazione non riconosciuto in fase di
  design**.

## Tentativo 4 — Tubo termoretraibile + inserto, verso il coil 19 Fr preformato

- Per i **prossimi campioni** si vuole tornare a usare il **coil 19 Fr preformato** (anziché il
  coil da piattella avvolta manualmente). Questo non è compatibile con l'**anello di PU**
  usato nel Tentativo 3 per l'accoppiamento dei mandrini, a causa del rigonfiamento che impedisce
  il passaggio delle spire già preformate.
- A seguito della **lacerazione del setto** riscontrata sulla cannula del Tentativo 3, il difetto
  è stato individuato alla **fine della cava** del **mandrino aspirazione** (nella zona di
  separazione dei due mandrini): in quel punto era stato erroneamente creato uno **spazio
  eccessivo**. Introdotto un **inserto** per **riempire** tale spazio in eccesso: correzione resa possibile dal
  fatto che il tubo PTFE ricopre il mandrino insieme all'inserto. Anche questo aspetto verrà
  corretto a monte con il nuovo design dei mandrini.
- Per l'accoppiamento dei mandrini, adottato un approccio intermedio con un **tubo
  termoretraibile** al posto dell'anello di PU:
  1. Il tubo termoretraibile è stato applicato sulla **parte terminale del mandrino reinfusione**,
     in corrispondenza della **porta di reinfusione** della cannula (circa 6 cm dalla punta) —
     punto dove il mandrino reinfusione termina. Questo punto è **distinto** dalla zona di
     divisione dei due mandrini, che si trova più in **zona prossimale**, prima che i due
     lumi/tubi diventino manicotti/raccordi.
  2. È stata dippata inizialmente solo la **parte prossimale** (lato manicotti/raccordi),
     fermandosi appena dopo la **zona di divisione dei due mandrini** (zona prossimale, vicino
     ai connettori).
  3. **Obiettivo**: la struttura in PU così ottenuta sulla parte prossimale doveva **mantenere
     i due mandrini in posizione accoppiata** anche dopo la successiva **rimozione del tubo
     termoretraibile**.
  4. Solo dopo la rimozione del termoretraibile si è proceduto a dippare la **parte distale** dei
     mandrini (punta della cannula), con l'obiettivo di poter usare il coil 19 Fr preformato
     senza più l'ostacolo del rigonfiamento.
- **Reinfusion port**: realizzata su questo campione rimuovendo lo strato di PU in corrispondenza
  della fine del mandrino reinfusione.

### Esito

- **Estrazione dei mandrini**: agevole. Il **PTFE ha aderito meglio** ai mandrini grazie a una
  leggera ottimizzazione del processo di stiramento/riscaldamento del tubo PTFE — il processo
  resta comunque **da ottimizzare ulteriormente**.
- **Accoppiamento mandrini**: una volta rimosso il tubo termoretraibile, i due mandrini si sono
  **leggermente disaccoppiati** nel punto dove finisce il mandrino di reinfusione, con un
  conseguente **aumento del diametro esterno** in quel punto. Anche in questo caso l'aumento di
  diametro ha **impedito l'uso del coil 19 Fr preformato**: è stato quindi necessario, ancora una
  volta, ottenere il coil da una **piattella in acciaio avvolta direttamente lungo il corpo della
  cannula**, anziché preformata.
- **Setto**: il campione **non presenta fori nel setto** — **conforme**, nessuna comunicazione
  tra i due lumi.
- **Sezione della porzione dual lumen**: **fuori specifica**, perché il PTFE sul mandrino
  aspirazione spinge il mandrino reinfusione verso l'esterno.

## Decisioni e prossimi passi

- **Confermata la scelta del dipping** per ottenere la porzione bilume della cannula, senza
  passare all'estrusione (vedi [Scelta tecnologica: dipping vs estrusione](#scelta-tecnologica-dipping-vs-estrusione)).
- **Design dei mandrini da rivedere**, per migliorare l'accoppiamento tra mandrino aspirazione e
  mandrino reinfusione e per tenere in considerazione la presenza del tubo in PTFE, che aumenta
  il diametro dei mandrini.
- **Deciso insieme al cliente**: si prosegue con il **tubo in PTFE stirato** come soluzione per
  l'estrazione dei mandrini; **sospesi, per il momento, i test sui mandrini con PTFE permanente**
  (teflonatura permanente, Tentativo 1).

## Collegamenti

- Progetto trasversale **PTFE-spray** (vedi [LINKS.md](../LINKS.md)) — approfondimenti sul
  confronto tra spray PTFE medical-grade come release agent.
