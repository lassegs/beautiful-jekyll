---
id: 310
title: '04.09.2014 &#8211; Geografiske representasjoner'
date: 2014-09-04T14:45:41+00:00
author: lassegs
layout: post
guid: http://skole.lassegs.org/?p=310
permalink: /2014/09/04/04-09-2014-geografiske-representasjoner/
wip_template:
  - full
image: /wp-content/uploads/sites/3/2014/09/Minard.png
categories:
  - SGO1910
---
<div>
  Foreleser: Andreas Forø Tollefsen
</div>

<div>
</div>

<div>
  Undervisningsplanen er oppdatert med tema og pensum til hver forelesning. Leveringer til besvarelser gjøres via Fronter.
</div>

<div>
</div>

<div>
  Forrige forelesning snakket vi om kart, grunnleggende prinsipper for kartdesign, grunnleggende kartografi. I dag går vi videre på dette:
</div>

<div>
</div>

  * Hva kan vi representere?
  * Hva vil vi representere?
  * Digitale representasjoner
  * Nøyaktighet
  * Objekter og attributter
  * Vektor og raster
  * Generaliseringer
  * Eksempler

<!--more-->

<div>
  Litt av motivasjonen er at verden er uendelig kompleks. Du kan zoome for alltid. Det er alltid en mulighet for å oppnå en enda større detaljrikdom. Vi må sette begrensning fordi systemene ikke klarer å vise verden akkurat som den er. Vi må velge hva vi ønsker å vise, vi må velge hvor mange detaljer, og velge hvilket tidspunkt vi vil visualisere. Vi har mange metoder for å visualisere. Vi har store datamengder, men begrenset plass.
</div>

<div>
</div>

<div>
  <strong>For å løse dette problemet gjør vi utvalg, samples. Vi kan ikke ta med alle, gjøre utvalg for å få med noen, som er representative for fenomenet vi ønsker å snakke om. Vi må også forenkle, generalisere, virkeligheten for å sette den inn i en datamodell.</strong>
</div>

### Hva kan vi representere?

<div>
  Hva vi representerer, henger sammen med hva vi mener eksisterer. Ikke bare fysiske ting, men også sosiale fenomer etc. Henger sammen med ontologi.
</div>

> <div>
>   &laquo;What is real, and exists, unconditionally&raquo;
> </div>
> 
> <div>
>   (Liedman1993; s.242)
> </div>

<div>
</div>

<div>
  Kan vi representere all heterogenitet? Vi må gruppere de inn i større grupper. Vi må generalisere variasjonen til et akseptabelt nivå (minioritet, klasse, objekter, grupper). Dette er en av hovedkritikkene mot GIS, at heterogenitet blir generalisert og minioriteter kan måtte vike for majoriteten.
</div>

<div>
</div>

<div>
  Hva kan ikke representeres eller hva er problematisk å representere geografisk.
</div>

<div>
</div>

<div>
  <div id="attachment_311" style="width: 459px" class="wp-caption alignnone">
    <a href="https://i0.wp.com/skole.lassegs.org/wp-content/uploads/sites/3/2014/09/Minard.png"><img class="wp-image-311 size-large" src="https://i0.wp.com/skole.lassegs.org/wp-content/uploads/sites/3/2014/09/Minard.png?resize=449%2C304" alt="I kartet over vises både tid, geografisk forflytning over tid, temperatur, troppstørrelse. Spatio-temporal eller rom-tid visualiseringer. Når man snakker om 3D-modeller trenger ikke den 3. dimensjonen være høyde. I GIS kan det være tid, eller andre atributter." srcset="https://i0.wp.com/skole.lassegs.org/wp-content/uploads/sites/3/2014/09/Minard.png?resize=449%2C304 449w, https://i0.wp.com/skole.lassegs.org/wp-content/uploads/sites/3/2014/09/Minard.png?zoom=2&resize=449%2C304 898w, https://i0.wp.com/skole.lassegs.org/wp-content/uploads/sites/3/2014/09/Minard.png?zoom=3&resize=449%2C304 1347w" sizes="(max-width: 449px) 100vw, 449px" data-recalc-dims="1" /></a>
    
    <p class="wp-caption-text">
      I kartet over vises både tid, geografisk forflytning over tid, temperatur, troppstørrelse. Spatio-temporal eller rom-tid visualiseringer. Når man snakker om 3D-modeller trenger ikke den 3. dimensjonen være høyde. I GIS kan det være tid, eller andre atributter.
    </p>
  </div>
</div>

<div>
</div>

### Hvordan representerer vi ting?

<div>
  Grunnleggende sanseoppfatning. I sinnet vårt oppfatter vi informasjon. Vi ser ting, hører lyder, lukter noe. Lagres i hjernen og kan brukes senere. Fotografier, lys fanget av linse. Kunst eller malerier. Fysiske modeller, arkitetmodeller. Talte og skriftelige beskrivelser. Eller gjennom målinger av den fysiske verden, distanser, områder, forskjellige attributter.
</div>

<div>
</div>

<div>
  De representasjoner som vi gjør forsterkes av regelr og lover vi har lært at gjelder. Vi kan observere et fallent tre, og kan vite at det engang har stått oppreist, og en gang kun var et lite frø. Slik kan vi bruke observasjoner og representasjoner til å <strong>predikere framtidige hendelser</strong>, basert på vitenskapelige lover og regler. Interpellere framtidig data, basert på data vi har i dag. En viktig del av romlig analyse (spatial analysis).
</div>

<div>
</div>

### Likheter kan modelleres og predikeres

<div>
  Toblers første geografiske lov:
</div>

> <div>
>   &laquo;Everything is related to everything else, but near things are more related than distant things.&raquo;
> </div>

<div>
  Jobber vi med vegetasjon, vet vi at vi kan gå en meter og anta at vegetasjonen er ganske lik der. Det samme med inntekt, at de husholdninger som er i nærheten av en husholdning med høy inntekt sannsynligvis også har høyere inntekt. Dette gjelder for all romlig data.
</div>

<div>
</div>

<div>
  Dette relaterer til romlig interpellasjon, der vi kan beregne det vi ikke har data for. Tenk på temperatur. Vi kan ikke måle temperatur overalt, men på enkelte målingstasjoner, og så sette en algoritme på det for å beregne temperaturen mellom stasjonen. Dess flere samplingspunkter, dess høyere resolusjon og nøyaktighet. Vi må gjøre både beregning og predikasjon for å få det fulle bildet av det vi studerer.
</div>

### Digitale representasjoner

<div>
  Kommer fra latin digit, latinsk for fingre, base 10 (decimal digit). Egentlig snakker vi om binære representasjoner, 1er og 0er.
</div>

<div>
  I dag vet vi stadig mer om hvordan digitale representasjoner som brukes.
</div>

<div>
  Vi bruker forskjellige standarder for forskjellige representasjoner.
</div>

  * Mp3 for musikk
  * jpeg for bilder
  * Flere formater i GIS for linke tid, rom og attributter sammen.

<div>
  Digitale representasjoner er mer effektive og billigere enn analoge representasjoner. Digital data kan representere uten menneskelig påvirkning.
</div>

<div>
  Digitale representasjoner har også fordelen av kompatibilitet og skala-økonomi. Enkelt. Trygt. Lett å bake up. Kompakt.
</div>

<div>
</div>

<div>
  Hvorfor trenger vi å vite om Bits og Bytes. I ArcGIS, integers (hele tall) blir lagret som
</div>

<div>
  kort integer (2 byet = 16 bit), som går mellom -65535 til +65 535
</div>

<div>
  Lang integer (4 byte = 32 bit), tall som mellom -4 294 967 925 til + 4 294 967 925
</div>

<div>
  Når vi legger data inn i GIS attributt-tabeller, må vi definere datatype for hver kolonne (variabel). Hver kolonne kan kun lagre en type data.
</div>

<div>
  Men ikke alle tall er hele tall (integers). Desimaltall lagres enten som FLOAT (single precision) eller DOUBLE (double precision)
</div>

<div>
</div>

<div>
  Vi kan også lagre tekst i en kolonne. Når vi lager en tekstkolonne må vi spesifisere hvor mange bokstaver kolonnen kan lagre.
</div>

<div>
</div>

<div>
  Vi bryr oss om dette fordi vi kan spare mye plass for å gjøre dette. Men også for å unngå problemer ved å matche variabler, for å jobbe med statistikk og lignende. Uten riktig ID blir det fort problemer.
</div>

<div>
  Når man skal importere fra Excel, må vi huske på at ArcGIS behandler alle celler som DOUBLE (double precision). Tekst vil bli lest som tekst, dato som dato.
</div>

### Representasjoners nøyaktighet

<div>
  Ingen representasjoner kan sies å være perfekte &#8211; bare så gode som vår data.
</div>

<div>
  Detaljer kan være irrelevant for projektet vårt, for dyrt å hente inn, eller kan kreve ekstrem datalagring og -behandling.
</div>

<div>
  Derfor er det veldig viktig å reflektere rundt hva som er utelatt og hva som er ignorert i vår data. Det er alltid mer i rommet, enn det den dataen vår forteller. Representasjoner kan også gjøre oss usikre, siden den ikke representere hele &laquo;realiteten&raquo;.
</div>

<div>
</div>

<div>
  <strong>Det fundamentale problemet</strong> er at verden er uendelig kompleks, mens datasystemer er begrensede. Geografiske data kobler rom og tid til en beskrivende egenskap ved dette stedet. Stedet blir registrert, og attributter blir assossiert med den registreringe (Type, status, startdato, sluttdato).
</div>

<div>
</div>

<div>
  Rader og kolonner. Hver rad er en enhet som vi er interessert i. Hver rad representerer et objekt, et &laquo;record&raquo;, i tabellen. Hver kolonne representerer en egenskap, og starter gjerne med XY-koordinat.
</div>

<div>
  Records lagres i rader, mens attributter lagres kolonner. Hver kolonne har en type data.
</div>

<div>
</div>

<div>
  Records = observations/cases/feature &#8211; rows, rader. En rad for hver feature.
</div>

<div>
  Attributes = variabler &#8211; kolonner.
</div>

### Hvordan registrerer vi attributter?

<div>
  Målenivå. Dette er viktig og vi husker det sikkert fra kvantitativ metode. Vil du kalkulere og beregne på disse dataene, må dette være riktig og huskes på.
</div>

<div>
</div>

<div>
  <strong>Nominalskala:</strong> Klassifikasjon basert på navn eller distinkte kategorier som ikke kan rangeres. De er &laquo;mutually exclusive&raquo; og uten rang. For eksempel farger eller stedsnavn. De sier noe om egenskapene ved objektet, men ikke noe om størrelse eller lignende. Land-type, trær, gress, etc. Kommunenummer. Bruker vi navn kan vi fort få duplikater. Mange steder heter London, f. eks, og dermed trenger vi mer informasjon, f. eks. fylke elller kommune.
</div>

<div>
  <strong>Ordinalverdier:</strong> Også en klassifisering med distinkte kategorier, men kan rangeres. Det kan være dikotomiske kategorier, f. eks syk/frisk. Eller ikke-dikotomiske som stor/medium/liten eller veldig fornøyd/litt fornøyd/ikke fornøyd.
</div>

<div>
  <strong>Intervallverdier: </strong>Konstante intervaller mellom verdier, men ikke en rate mellom. Vi kan ikke si at 20 C er to ganger så varmt som 10 C.
</div>

<div>
  <strong>Ratioverdier: </strong>Konstante intervaller med en absolutt null.
</div>

<div>
  <strong>Sykliske verdier: </strong>Månedene i et år, kompassretning.
</div>

### Hva med objektene?

<div>
  To fundamentalt forskjellige måter for å forstå geografi:
</div>

<div>
  Forstå og representere geografisk data som diskre data &#8211; definerte grenser
</div>

<div>
  Forstå og representere geografisk data som fortsettende felt.
</div>

<div>
</div>

<div>
  <strong>Vektor: </strong>
</div>

  * Diskre objekter med klart definerte grenser
  * Punkt, linjer og polygoner.
  * Attributter med informasjon

<div>
  <strong>Raster:</strong>
</div>

  * Fortsettende felt.
  * Pikselverdier representerer informasjon.
  * En verdi pr piksel.

<div>
  <strong>Diskre objekter</strong>
</div>

<div>
  Det er generaliseringer ved bruk av polygoner. En forenklet representasjon av det ekte objektet. Fordi du må ha uendelig antall noder for å lage en perfekt sirkel.
</div>

<div>
</div>

<div>
  <strong>Fortsettende felt</strong>
</div>

<div>
  Ikke-diskre objekter, ikke fiksert i rom, men varierer fortsettende gjennom rommet.
</div>

<div>
  Høyde er et bra eksempel. Hele jordas overflate har høyde, men det varierer. Populasjon kan også være det.
</div>

<div>
  Raster (grid cells), rektangulær &#8211; vanligvis firkantede celler, hvor geografisk variasjon er representert ved å bruke verdier for hver celle.
</div>

<div>
  Effekter av raster representasjon ved bruk av a) den største andelen-regelen og b) det sentrale punktet. Det gir forskjellige outputs.
</div>

<div>
</div>

> <div>
>   &laquo;Raster is faster, but vector is corrector&raquo;
> </div>
> 
> <div>
>   -Tollefsen
> </div>

### Intern variasjon

<div>
  Felles for både diskre objekter og rasterdata er at de begge ignorerer eller skjuler intern variasjon. Vi må enten akseptere homogen representasjon, eller velge hva vi vil representere.
</div>

<div>
</div>

<div>
  Vi generaliserer for forenkle representasjonene. Men vi må alltid forenkle den komplekse virkeligheten for å lage en representasjon. Og det må vi huske på.
</div>

<div>
</div>

<div>
  <em>Foto: Wikimedia</em>
</div>