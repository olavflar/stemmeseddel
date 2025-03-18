# Stemmeseddel-prosjekt

## Problemstilling
Under generalforsamlinger i borettslag eller sameier er det normalt en tidskrevende, manuell prosess å finne ut av hvem som er stemmeberettiget og å fordele stemmesedler basert på eierandeler. Styret må håndtere køer, håndtere lister, og forsikre seg om at kun riktige personer får utdelt stemmesedler med korrekt vekt. Dette skaper ofte lange ventetider, risiko for feil og frustrasjon blant beboere.

Foreslått løsning
Vi skal digitalisere prosessen ved å:

Opprette et registreringsskjema (Google Forms) der beboere fyller inn relevant informasjon (navn, leilighetsnummer, kontaktinfo).
Automatisere kontroll mot styrets register (Google Sheets) via et Google Apps Script. Scriptet vil bekrefte at beboeren faktisk hører til leilighetsnummeret, og samtidig hente eierandelen knyttet til denne leiligheten.
Tildele stemmeseddel automatisk basert på aksjeandel og generere en QR-kode som beboeren kan motta på e-post. Ved oppmøte skannes denne QR-koden for raskt å bekrefte identiteten og stemmevekten, slik at riktig (fargekodet) stemmeseddel kan deles ut.
Opprette et admin-dashboard (Google Sheets) for styret, hvor man kan se en oversikt over:
Hvor mange som har registrert seg.
Hvem som er bekreftet og har mottatt QR-kode.
Hvem som trenger manuell gjennomgang.
Logger og tidspunkt for hver godkjenning.
Opsjon på PDF-stemmesedler, hvis ønsket. Man kan bruke et script (Google Apps Script eller Python) for å generere PDF-filer som viser navn, leilighetsnummer, aksjeandel og eventuell fargekode for stemmeseddelen.
Resultat

Redusert tidsbruk: Beboere slipper å stå i lange køer, og styret slipper å bla i papirlister.
Færre feil: Riktig aksjeandel og identitet blir sjekket automatisk.
Bedre oversikt for styret: Styret ser i sanntid hvor mange som er bekreftet og hvem som eventuelt må sjekkes.
Enklere kvitteringsmekanisme: Ved QR-kode-skanning får beboeren enkelt ut riktig fargekodet stemmeseddel, og styret har oversikt over hvem som har hentet.
Denne løsningen er lett å implementere, krever lite ekstra infrastruktur og kan deretter utvides etter behov (f.eks. digital stemmeinnlevering, live-resultater eller integrasjon med andre systemer).
Kode for å automatisere generering av stemmesedler ved generalforsamling.  
Bruker Google Sheets, Google Apps Script og Python for QR-kodegenerering og PDF-eksport.

## Funksjoner
- Google Forms-registrering
- QR-kode for bekreftelse
- PDF-stemmesedler med fargekoding
- Automatisk e-postutsendelse

## Kom i gang
1. Klon repoet: `git clone <repo-URL>`
2. Installer nødvendige pakker: `pip install -r requirements.txt`
3. Sett opp Google Apps Script-prosjektet, etc.

## Lisens
[MIT License](LICENSE)
