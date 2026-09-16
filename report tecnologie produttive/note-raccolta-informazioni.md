# Note raccolta informazioni — Report di tecnologie produttive individuate

> Materiale grezzo raccolto in conversazione, da usare come base per la stesura del report finale
> "Report di tecnologie produttive individuate". Non ancora rielaborato in forma di report.

## Contesto progetto

- Progetto per la realizzazione di un prototipo di **cannula dual lumen per ECLS**.
- La cannula non è bilume su tutta la lunghezza: comprende una porzione a **singolo lume** vicino
  alla punta. Il **lume di reinfusione termina circa a metà cannula**. I due lumi confluiscono in
  **due raccordi separati**.

## Attività 1 — Reverse engineering (completata)

- Analisi della cannula bilume competitor **Avalon Elite 19 Fr**
  (https://www.getinge.com/it/prodotti/catetere-avalon-elite).
- Report già prodotto, si trova in `report reverse engineering/`.

## Attività 2 — Tecnologie produttive individuate (oggetto di questo report)

Le tecnologie individuate riguardano **tutta la cannula**, non solo il tratto bilume.

### Scelta tecnologica: dipping vs estrusione

- Ci si è concentrati sulla tecnologia del **dipping**, in contrapposizione all'**estrusione**,
  per sfruttare l'esperienza pregressa maturata negli anni.
- La scelta dipping vs estrusione è **ancora aperta**, non definitiva.
- In parallelo, è stato richiesto anche un **prototipo per estrusione** di un tubo bilume in
  poliuretano tramite **fornitore esterno**, dato che l'estrusione richiede macchinari dedicati
  non disponibili internamente.

### Processo di dipping — panoramica generale

Per ottenere la cannula bilume per dipping:

1. Due **mandrini** (uno per il lume di aspirazione, uno per il lume di reinfusione), accoppiati
   in qualche modo.
2. **Immersioni ripetute** in soluzione di **poliuretano + THF** → strato base di poliuretano sui
   mandrini.
3. Deposizione di un **coil in acciaio** sopra lo strato base, per la resistenza meccanica.
4. **Strato esterno** di poliuretano, per dipping o per laminazione.
5. **Rimozione dei mandrini**.

### Problema principale del dipping

Il problema principale del dipping (non specifico alla dual lumen, ma generale a tutte le
cannule prodotte con questa tecnologia) è l'**estrazione dei mandrini** una volta evaporato il THF.

## Estrazione mandrini — soluzione validata su cannule monolume

Per le cannule monolume già realizzate in passato:

- Si stira un **tubo in PTFE** sul mandrino, applicando una **temperatura di circa 400°C** e una
  **trazione di 5 kg**.
- Il tubo in PTFE, ricoperto di poliuretano, viene **intestato (rifinito) in cima e in fondo** al
  mandrino.
- Si riesce a sfilare il mandrino perché **il PTFE non si attacca all'acciaio** del mandrino.
  Il **poliuretano invece si aggrappa tenacemente all'acciaio**, rendendo l'estrazione diretta
  molto difficile, se non impossibile, senza l'interposizione del PTFE.
- **Passaggio finale**: estrazione del PTFE dall'interno del tubo in poliuretano — manovra
  abbastanza agevole. Si afferra il PTFE con una pinza e si **torce/tira** fino al completo
  distacco dal tubo in poliuretano ottenuto.

## Geometria dei mandrini bilume — la sfida specifica

- Il **mandrino aspirazione** presenta una **cava** (concavità marcata) che alloggia il mandrino
  di reinfusione.
- Il processo di **stiratura del tubo PTFE** (validato sui mandrini monolume) **non riesce ad
  aderire nella parte concava** del mandrino di aspirazione.

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
  (uno **verde**, uno **nero**), con superficie **molto più liscia** rispetto ai mandrini dual
  lumen trattati dal fornitore esterno. Usati per realizzare due cannule monolume: entrambe si
  sono staccate.
  - ⚠️ **Da confermare**: il distacco sul mandrino nero è avvenuto con molta difficoltà; non è
    certo che entrambe le cannule si siano staccate facilmente.

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
  permanentemente (superficie rugosa), realizzata una cannula bilume completa.
  **Esito negativo**: dopo la maturazione del PU, l'estrazione **non è stata comunque possibile**.
  Rimossi i mandrini tagliando PU e coil (non sciolto nel THF, per poter ispezionare i residui).
  **Riscontro**: superficie interna della cannula **piena di residui di PTFE** — non accettabili
  per questa cannula.
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
- **Mandrino aspirazione**: il PTFE ha formato inizialmente una **membrana tesa** sulla parte
  concava. Lavorata manualmente (a caldo e a freddo), spingendola dentro la cava.
  **Esito positivo**: la membrana si è deformata a sufficienza per aderire anche nella zona
  concava.

### Processo di dipping stratificato (formazione del setto)

1. **Dipping del mandrino reinfusione da solo** → primo strato base.
2. **Accoppiamento** del mandrino reinfusione (con il suo primo strato base) al mandrino
   aspirazione.
3. **Dipping di entrambi i mandrini insieme** → strato base della cannula finale.
4. Risultato: il mandrino reinfusione ha un **doppio strato base** (spessore maggiore).
5. Il **primo strato base del mandrino reinfusione**, nella zona tra i due mandrini, **funge da
   setto** della porzione bilume della cannula finale.

> Punto aperto per sviluppi futuri: il fatto di aver dippato solo il mandrino reinfusione prima
> dell'accoppiamento potrebbe essere rivisto — forse sarà necessario dippare anche il mandrino
> aspirazione prima di accoppiarlo.

### Prima cannula bilume completa con questo processo

- **Estrazione dei mandrini riuscita** — problema critico di estrazione risolto.
- **Analisi della cannula**: rilevata una **lacerazione del setto** tra i due mandrini, nel punto
  dove questi si dividono (vicino alla zona dei connettori). La lacerazione **mette in
  comunicazione i due lumi** — **difetto critico, non accettabile**.
- **Ipotesi di causa**: rottura forse dovuta a uno **scarso accoppiamento** dei due mandrini in
  quella zona, riconducibile a un **difetto del mandrino aspirazione non riconosciuto in fase di
  design**.

## Azione correttiva in corso

- Nuova cannula dual lumen in fase di realizzazione.
- Introdotto un **inserto** nella **zona di separazione dei due mandrini**, posizionato nella
  **cava** che ospita il mandrino reinfusione.
- L'inserto viene **inglobato nel tubo PTFE insieme al mandrino aspirazione** — soluzione
  ritenuta accettabile.
- **Stato**: in attesa dell'esito della nuova cannula.

## Collegamenti

- Progetto trasversale **PTFE-spray** (vedi [LINKS.md](../LINKS.md)) — approfondimenti sul
  confronto tra spray PTFE medical-grade come release agent.
