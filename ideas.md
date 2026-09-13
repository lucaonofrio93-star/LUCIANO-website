# Direzione creativa — Dott. Luciano Onofrio

## Tre possibili approcci

| Tema | Breve introduzione | Probabilità |
|---|---|---:|
| Archivio Clinico Italiano | Un linguaggio editoriale, silenzioso e preciso: carta avorio, blu d’inchiostro e gerarchie tipografiche misurate. Trasmette cura senza ricorrere ai codici ospedalieri o alle convenzioni dei template medici. | 0,07 |
| Giardino della Fiducia | Una composizione più organica, con verdi soffusi, luce naturale e dettagli ispirati all’architettura di uno studio privato. Calda e prossima, senza perdere autorevolezza. | 0,04 |
| Segnale Notturno | Una direzione scura e contemporanea, incentrata sul contrasto tra blu profondo e informazioni funzionali molto chiare. È più urbana e tecnologica, perciò meno adatta al tono discreto richiesto. | 0,08 |

## Approccio selezionato: Archivio Clinico Italiano

### Movimento di design

Il progetto adotta un **editorial minimalism contemporaneo** con richiami alla modulistica sanitaria privata e all’eleganza materica della carta da corrispondenza. Non è una riproduzione storica: usa precisione, margini, linee sottili e ritmo tipografico come strumenti di fiducia.

### Principi guida

1. Le informazioni essenziali vengono prima dell’ornamento: telefono, posizione, orari e qualifiche sono sempre riconoscibili.
2. Il bianco caldo non è uno sfondo neutro ma uno spazio di respiro, con superfici in avorio e dettagli in carta leggermente più scura.
3. La composizione è asimmetrica e sequenziale, come un fascicolo ben ordinato, mai una raccolta di card identiche.
4. La discrezione è parte dell’esperienza: i feedback sono tattili e leggeri, senza pop-up, badge invasivi o animazioni spettacolari.

### Filosofia cromatica

La base avorio attenua la freddezza tipica delle interfacce cliniche e comunica accoglienza. Il blu notte è il colore della competenza e strutturerà titoli, footer e punti decisionali; il teal smorzato verrà usato solo per riconoscere azioni operative e dettagli di stato. Il colore firma sarà **Blu Inchiostro Faicchio** (`#113A5B`), un blu pieno e sobrio che caratterizza pulsanti, micro-elementi e navigazione.

### Paradigma di layout

La pagina segue una **colonna editoriale laterale**. Sul desktop, un margine verticale guida lo sguardo attraverso marcatori di sezione, invece di chiudere ogni argomento in una griglia uniforme. L’hero bilancia una colonna di testo con una superficie di immagine o texture; le pagine interne mantengono un’intestazione d’archivio e un contenuto disposto in fasce. Su mobile la sequenza diventa una colonna nitida e molto leggibile, con accesso persistente alle azioni.

### Elementi firma

Il sito usa un filettino verticale in teal come marcatore di percorso, numerazioni di sezione discrete e una trama di micro-punti carta appena percettibile sulle superfici avorio. Le carte informative hanno angoli quasi netti e una singola tacca grafica, per evocare schede ordinate invece del consueto effetto “pill”.

### Filosofia delle interazioni

Ogni interazione deve confermare una scelta, non attirare attenzione. I pulsanti si comprimono impercettibilmente al tocco e cambiano con contrasti netti; i link testuali espandono una sottolineatura teal. Il menu mobile si apre come un pannello di consultazione con focus gestito, mentre la galleria consente una visione ravvicinata senza interrompere l’orientamento nella pagina.

### Animazione

Le transizioni usano esclusivamente opacità e trasformazioni, con una curva di uscita rapida `cubic-bezier(0.23, 1, 0.32, 1)` e durate tra 140 e 260 ms. Gli ingressi di sezione sono piccoli scorrimenti verticali con opacità crescente e il contenuto a gruppi è sfalsato con ritardi di 50 ms. Tutto il movimento non essenziale viene disattivato in presenza di `prefers-reduced-motion`.

### Sistema tipografico

I titoli useranno **DM Serif Display**, con grazie misurate e professionali, mentre il testo operativo userà **Manrope** per precisione e leggibilità sugli schermi piccoli. Le maiuscolette tracciate identificano metadati e marcatori; H1 rimane importante ma non enfatico, H2 costruisce il ritmo e il corpo conserva una misura di lettura confortevole.

### Essenza del brand

**Uno studio di chirurgia generale e colonproctologia per chi cerca un orientamento specialistico chiaro, riservato e facilmente accessibile a Faicchio.** La personalità è **misurata, competente, rassicurante**.

### Voce del brand

I titoli sono diretti e sobri; le CTA spiegano l’azione reale invece di usare formule promozionali. La microcopy evita superlativi e promesse cliniche.

> «Competenza specialistica, attenzione alla persona.»

> «Per fissare un appuntamento, contatti direttamente lo studio.»

### Wordmark e logo

Non verrà creato né ridisegnato un logo del medico. L’header prevede un’area per il **logo autentico** se fornito o rintracciato nella scheda dell’attività; fino a quel momento mostra soltanto un segno decorativo non identificativo e il nome testuale, senza dichiararlo come marchio ufficiale. La favicon sarà attivata solo a partire da un asset ufficiale autorizzato.

## Decisioni operative sugli asset

Le immagini in primo piano saranno esclusivamente fotografie reali e autorizzate dello studio o del medico. In loro assenza, il progetto impiegherà uno sfondo astratto non figurativo a bassa intensità, dichiarato nel codice come fallback temporaneo; non verranno mai generati ritratti, ambienti sanitari simulati, fotografie di medici terzi o un logo sostitutivo.
