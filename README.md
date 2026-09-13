# Sito web — Dott. Luciano Onofrio

## Scopo della versione

Questo progetto è un sito statico in React e TypeScript per presentare il Dott. Luciano Onofrio e facilitare il contatto diretto con lo studio. La prima versione usa chiamata telefonica e link esterni a Google Maps; non contiene un modulo di contatto, sistema di prenotazione online, raccolta di dati sanitari o integrazioni di analytics attivate.

## Dati centralizzati

Tutte le informazioni operative sono raccolte in `client/src/data/business.ts`. Per aggiornare numero di telefono, indirizzo, orari, valutazione, numero di recensioni, URL Google Maps, ambiti, prestazioni o asset, modificare quel file e non i singoli componenti.

| Informazione | Posizione | Regola |
|---|---|---|
| Nome, telefono, indirizzo e URL Maps | Oggetto `business` | Verificare con il titolare o con la scheda Google Maps prima di ogni modifica. |
| Orari | Array `openingHours` | Aggiornare i giorni di chiusura tramite `closed: true`. |
| Valutazione Google | `rating` e `reviewCount` | Ricontrollare entrambi i valori insieme e mantenere il collegamento alla fonte. |
| Ambiti e prestazioni | `specializationAreas` e `services` | Inserire solo elementi esplicitamente confermati. |
| Galleria | Array `galleryItems` | Inserire unicamente file originali e autorizzati. |
| Texture astratte | Oggetto `visualFallbacks` | Sono decorative e non rappresentano il medico, lo studio o un presidio sanitario. |

## Fotografie e logo

Il progetto non include fotografie del medico, fotografie dello studio o un logo ricreato. La scheda Google Maps mostra elementi fotografici, ma il loro riuso sul sito deve essere autorizzato dal titolare. Una volta ricevuti i file originali, conservarli fuori dal repository nella directory `/home/ubuntu/webdev-static-assets/`, caricarli nella libreria asset del progetto e usare gli URL restituiti nella configurazione.

Per attivare la galleria, inserire gli elementi nell’array `galleryItems` nel seguente formato:

```ts
{
  src: "/manus-storage/foto-studio-esempio.webp",
  alt: "Descrizione accurata della fotografia reale dello studio",
  caption: "Facoltativa"
}
```

L’interfaccia abilita automaticamente griglia su desktop, scorrimento adattivo, caricamento differito e lightbox accessibile. L’area logo nell’header è volutamente testuale fino alla fornitura di un asset ufficiale; la favicon dovrà essere attivata soltanto da un file ufficiale confermato.

## Privacy e pubblicazione

Le pagine `Privacy Policy` e `Cookie Policy` sono strutture informative e non sostituiscono una valutazione legale. Prima della pubblicazione, il titolare dovrà verificare e completare titolare del trattamento, recapiti per l’esercizio dei diritti, provider di hosting, eventuali log tecnici, soggetti terzi e politiche effettivamente applicabili. Qualunque attivazione successiva di form, analytics, font esterni, widget, mappa incorporata o cookie non tecnici richiede un aggiornamento preventivo delle informative e, quando necessario, del consenso.

## Controlli prima del go-live

Prima della pubblicazione, verificare sempre che telefono, indirizzo, orari, URL Maps, rating e conteggio recensioni corrispondano alla fonte corrente. Testare inoltre tutte le CTA su smartphone, l’accesso da tastiera, l’apertura delle indicazioni e la presenza delle fotografie autorizzate. Il file `verified-source-notes.md` riporta il perimetro della ricognizione iniziale e gli elementi che richiedono conferma.
