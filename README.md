# Peak Conditions

## Kjøring av appen

For å kjøre appen må en skrive 'npm install' og deretter 'npm run dev'.

## Beskrivelse av appen

Peak Conditions skal gi brukerne en bedre måte å sjekke været på. Når en først går inn på siden, ser en destinasjoner og været på det laveste punktet til skistedet. Når en trykker på "detaljer", får en været akkurat nå på tre punkter og et langtidsvarsel for det laveste punktet. Hvis en trykker på en av de to andre punktene, vil langtidsvarselet gjelde for det punktet.

## Valg vi har tatt

Vi har antatt at en kan presentere ett kort om gangen i et rutenett (en form for liste), der scrolling gir muligheten til å bla seg frem eller tilbake. en hopper til en spesifikk ressurs ved å trykke på "detaljer" under kortet.

Vi har et filter der en kan sortere skistedene etter navn. en kan også velge å bare vise favoritter. Favoritter huskes når en lukker nettleseren din og åpner den igjen. Hvis en refresher siden, vil den huske om en filtrerer alfabetisk eller reversert alfabetisk, men hvis en laster inn siden på nytt, vil den filtrere alfabetisk.

Man kan trykke på stjernen på et destinasjonskort for å legge den til som favoritt. Dette valget huskes når en starter nettleseren på nytt.

Siden er responsiv, slik at appen kan brukes på både store skjermer og mindre smarttelefoner.

Et godt eksempel på ryddig utforming er langtidsvarselet for et skisted. Hvis en bruker mobil, endres presentasjonen av tabellen drastisk for å opprettholde en ryddig utforming.

## Tekniske prestasjon

Peak Conditions vil aldri sende flere forespørsler til Meteorologisk institutts API enn nødvendig. Appen sjekker når Meteorologisk institutt skal oppdatere værvarslingen for en destinasjon og holder dataen fersk helt frem til da.

## Hva som er testet

Siden dekningsgraden ikke var fokus for P1, har vi bare testet en komponent. 'DestinationCardComponent' har to vanlige komponenttester og en snapshot-test. Dataen er mocket slik at ingen API-kall blir gjort. For å kjøre testene, bruk 'npm test'.
