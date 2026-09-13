# Correzione hero landing

- [x] Identificare se la forma a destra proviene dal visual hero, dall’overlay CSS o da un overflow del layout.
- [x] Correggere la sovrapposizione mantenendo il fallback astratto non figurativo, senza coprire testo o CTA.
- [x] Verificare la hero a viewport desktop e mobile.
- [x] Eseguire typecheck/build e salvare un checkpoint della correzione.

## Vincolo di design

Preservare la direzione Archivio Clinico Italiano: texture avorio/blu, contrasto accessibile, segni editoriali discreti e nessuna fotografia non autorizzata.

## Riscontro iniziale

Nel rendering desktop la hero usa una colonna visuale destra con texture astratta, pseudo-elemento overlay e nota informativa in basso a destra. Il controllo dovrà distinguere il pannello intenzionale da eventuali elementi assoluti che fuoriescono o coprono il contenuto.

## Fonte

Segnalazione del committente: “c’è una forma sulla destra che copre della landing page”.

*Da completare dopo la verifica e la correzione.*
