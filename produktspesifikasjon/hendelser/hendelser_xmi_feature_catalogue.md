#### Felles

Overordnet informasjon.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>identifikasjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Unik ID.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>uuid</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>betegnelse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Navn eller beskrivelse av hendelsen.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>førsteRegistreringstidspunkt</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Dato og tid for førstegangs-registrering av hendelsen.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>DateTime</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>oppdateringstidspunkt</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Dato og tid for siste oppdatering.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>DateTime</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>geometriobjekt</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>referanse til en eksisterende geometri som stedefester dette objektet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>URI</td>
    </tr>
  </tbody>
</table>

#### ops

Egenskaper

(ingen)

Relasjoner

**Assosiasjoner**
Hendelse – rolle: hendelse – kardinalitet: 0..*
Ressurs – rolle: potesiellResserus – kardinalitet: 0..*

#### Helsesamvirke

Hendelsestype som ikke inngår i de forhåndsdefinerte hendelsestypene.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>samvirkeType</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeHelsesamvirke</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- firstResponder<br />- tvang</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Hendelse

#### Hendelse (abstrakt)

Forekomst eller endring i et bestemt sett med omstendigheter (NS-EN ISO 22300: 2021; NS-ISO 31000: 2018) og som nødetatene ser behov for å informere om.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>punkt</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Geografisk lokasjon for hendelsen.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Punkt</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>opphavsaktør</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Den enhet som registrerer eller rapporterer en hendelse, begrenset til politi, brann, helse eller HRS.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Hovedaktør</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- politi – Politi<br />- helse – Helse<br />- brann – Brann<br />- HRS</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>innmelder</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Person eller sensor som varsler om en hendelse til nødetatene.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Observatør</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>innmelder.kontaktinformasjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Kontaktinformasjon</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterStreng</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>innmelder.OPSoperatør</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Angir om operatøren er tilknyttet OPS.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>innmelder.sensor</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>om observasjonen er gjort fra en automatisk sensor.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>beskrivelse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Kort beskrivelse som fritekst.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>prioritet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>hvor høyt en hendelse prioriteres med hensyn til alvorlighet og hastegrad<br />Merknad: Avledes fra alle aktørenes vurdering av prioritet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>PrioritetHendelse</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- høy – Hendelse som krever umiddelbar respons (akutt)<br />- middels – Hendelse som krever rask respons<br />- lav – Hendelse som krever respons<br />- ingen – ingenPrioritet<br />- ikkeSatt – Prioritet ikke vurdert</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kompleksitet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>hvor krevende/komplisert det er å håndtere en hendelse<br />Merknad: Avledes fra alle aktørenes vurdering av kompleksitet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Kompleksitet</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- komplisert – Hendelser som er særlig utfordrende å håndtere, eksempelvis på grunn av sitt omfang, krav til spesialisert kompetanse, tilgjengelighet til hendelsessted og/eller krav til koordinering mellom nødetatene.<br />- rutine – Hendelser som ikke defineres som komplekse<br />- ikkeSatt – Hendelsens kompleksitet ikke vurdert</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>aktørPerspektiv</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Hendelsens prioritet og kompleksitet for en aktør.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>AktørPerspektiv</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>aktørPerspektiv.aktør</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>enhet som bidrar i å håndtere en hendelse, begrenset til politi, brann, helse eller HRS.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Hovedaktør</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- politi – Politi<br />- helse – Helse<br />- brann – Brann<br />- HRS</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>aktørPerspektiv.prioritet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Et uttrykk for hvor høyt en hendelse prioriteres med hensyn til alvorlighet og hastegrad.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>PrioritetHendelse</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- høy – Hendelse som krever umiddelbar respons (akutt)<br />- middels – Hendelse som krever rask respons<br />- lav – Hendelse som krever respons<br />- ingen – ingenPrioritet<br />- ikkeSatt – Prioritet ikke vurdert</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>aktørPerspektiv.kompleksitet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Et uttrykk for hvor komplisert det er å håndtere en hendelse.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Kompleksitet</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- komplisert – Hendelser som er særlig utfordrende å håndtere, eksempelvis på grunn av sitt omfang, krav til spesialisert kompetanse, tilgjengelighet til hendelsessted og/eller krav til koordinering mellom nødetatene.<br />- rutine – Hendelser som ikke defineres som komplekse<br />- ikkeSatt – Hendelsens kompleksitet ikke vurdert</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>lokalitetstype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Beskrivelse av omgivelsene der en hendelse finner sted.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Lokalitetstype</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>øvelse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Angir om hendelsen er en øvelse.<br />Merknad: Dersom egenskapen ikke angis, skal hendelsen betraktes som reell</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Felles

**Assosiasjoner**
ops – rolle: ops – kardinalitet: 1
Utbredelse – rolle: framskriving – kardinalitet: 0..*
Objekt – rolle: objekt – kardinalitet: 0..*
Utbredelse – rolle: utbredelse – kardinalitet: 0..*
Tiltakslokasjon – rolle: tiltakslokasjon – kardinalitet: 0..*
SammensattHendelse – rolle: sammensattHendlelse – kardinalitet: 0..1
Ressurs – rolle: tilordnetRessurs – kardinalitet: 0..*
Kontekst – rolle: kontekst – kardinalitet: 0..*
Observatør – rolle: innmelder – kardinalitet: 1..*

#### PlanlagtHendelse

Hendelse som nødetatene er kjent med og som i kraft av sitt omfang krever særskilte forberedelser.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>planlagtHendelsesType</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypePlanlagtHendelse</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- arrangement – Planlagte arrangementer, f. eks idrett, kultur, konserter, festivaler ol.<br />- demonstrasjon – Planlagte demonstrasjoner.<br />- VIP – Planlagte hendelser som krever særskilt beskyttelse av deltakere i hendelsen, eksempelvis grunnet deres offisielle status som myndighetspersoner.<br />- annenPlanlagtHendelse – Planlagt hendelse som ikke inngår i de forhåndsdefinerte kategoriene for slike hendelser.</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Hendelse

#### Utbredelse

Geografisk utbredelse av hendelsen.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>flate</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Geometri som avgrenser hendelsen dersom hendelsen kan defineres som en flate (eks. skogbrannområder og flomområder).</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Flate</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kurve</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Geometri som avgrenser hendelsen dersom hendelsen kan defineres som en kurve (eks. brannfront).</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Kurve</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>utbredelsestype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Spredningsbeskrivelser for et utvalg av hendelser som har begreper for utbredelse.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeUtbredelse</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- hendelsesområde – En generisk betegnelse for ustrekning av en hendelse som kan brukes dersom hendelsen ikke har begreper for områder som er rammet.<br />- brannfront – Den fremste delen av en brann hvor forbrenningen er mest intens og hvordan brannen sprer seg videre (retning, hastighet, tid, prognose, etc.).<br />- aktivtBrannområde – Området som er rammet av brannen, hvor det pågår aktiv brann.<br />- brentOmråde – Området som er rammet av brannen, som er brent.<br />- skredområde – Området som er rammet av skredet.<br />- flomområde – Området som er rammet av flommen.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>beskrivelse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Kort beskrivelse som fritekst.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Felles

#### SammensattHendelse

Sammenstilling av flere hendelser (f. eks. ekstremvær med mye nedbør i et helt vassdrag, hvor det oppstår hendelser i et helt dalføre).

Egenskaper

(ingen)

Relasjoner

**Arv**
Felles

**Assosiasjoner**
Hendelse – rolle: hendelse – kardinalitet: 0..*

#### AnnenHendelse

Hendelsestype som ikke inngår i de forhåndsdefinerte hendelsestypene.

Egenskaper

(ingen)

Relasjoner

**Arv**
Hendelse

#### Sikkerhetshendelse

Hendelser som er utløst av helt eller delvis villede handlinger og som medfører fare for omgivelsene, inkludert for nødetater. Hendelsestypen inkluderer ulovlige og straffbare handlinger.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>sikkerhetshendelseType</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeSikkerhetshendelse</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- vold – En hendelse der fysisk makt, trusler eller overgrep utøves mot en eller flere personer, med potensial for skade på liv og helse.<br />- orden – En hendelse som krever tiltak for å gjenopprette eller opprettholde offentlig ro og sikkerhet, ofte relatert til forstyrrelser, uro eller situasjoner som kan eskalere til vold eller skade.<br />- PLIVO – En pågående situasjon der en eller flere gjerningspersoner utøver, eller er i ferd med å utøve, livstruende vold mot flere uskyldige personer. Skadeomfanget er, eller vurderes å kunne bli, så stort at nødetatene raskest mulig må gå i ekstraordinær innsats sammen, for å stanse handlingene og redde liv (Nasjonal prosedyre – PLIVO).<br />- terror – Terrorhandling: Ulovlig bruk av, eller trussel om bruk av, makt eller vold mot personer eller eiendom, i et forsøk på å legge press på landets myndigheter eller befolkning eller samfunnet for øvrig for å oppnå politiske, religiøse eller ideologiske mål (NOU 2016: 19 Samhandling for sikkerhet).<br />- sabotasje – Sabotasje er å skade eiendom, produksjonsmidler eller tekniske systemer med hensikt (SNL).<br />- bombetrussel – En hendelse der det blir fremsatt en påstand eller mistanke om at en eksplosiv enhet er plassert, noe som utløser behov for evakuering, søk og vurdering av risiko.<br />- helserelatertSikkerhetssituasjon – Hendelser som involverer personer som kan utgjøre en fare for seg selv eller andre, eksempelvis knyttet til rus eller psykisk tilstand.<br />- annenSikkerhetshendelse – Sikkerhetshendelse som ikke inngår i de forhåndsdefinerte typene.</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Hendelse

#### Naturhendelse

Hendelse som er forårsaket av naturforhold

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>naturhendelseType</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Kategorier av hendelsestypen naturhendelse.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeNaturhendelse</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- skred – Masse (stein, løsmasser, leire, jord) som beveger seg nedover skråninger og/eller under vann (delvis basert på NVE m fl).<br />- snøskred – Masse (snø, våt eller tørr) som beveger seg raskt nedover en skråning (NVE m fl).<br />- flom – Vannføring som går ut over normale nivåer og som fører eller kan føre til skade på infrastruktur og/eller bebyggelse.<br />- skogGressMarkbrann – En brann som oppstår i vegetasjonsområder i innmark og utmark.<br />- ekstremvær – Vær som medfører fare for liv og verdier. Ekstremvær kan være sterk vind, kraftig nedbør, stormflo og høye bølger eller en kombinasjon av værelementer som til sammen utgjør en fare.<br />- annenNaturhendelse – Naturhendelse som ikke inngår i forhåndsdefinerte naturhendelsestyper.</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Hendelse

#### Ulykke

En ikke villet hendelse som forårsaker skade.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>ulykkeType</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeUlykke</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- trafikkulykke – Ulykker som skjer på veiene i forbindelse med forflytting av mennesker og gods. Det kan være møteulykker, utforkjøringer og skader på fotgjengere og syklister (SNL).<br />- jernbaneulykke – En uønsket eller utilsiktet plutselig begivenhet eller en bestemt rekke slike begivenheter som har skadelige følger, herunder som medfører at noen dør eller blir alvorlig skadet, som medfører betydelig skade på jernbanemateriell, på kjørevei, på eiendom utenfor jernbanen eller på miljø, og alle andre lignende ulykker (Jernbaneundersøkelsesloven § 5).<br />- tunnelulykkeVei – Veiulykke i tunnel.<br />- tunnelulykkeJernbane – Jernbaneulykke i tunnel (se jernbaneulykke).<br />- tunnelbrannVei – Brann i veitunnel.<br />- tunnelbrannJernbane – Brann i jernbanetunnel.<br />- bygningsulykke – En ulykke som involverer skade eller sammenbrudd av en bygning, inkludert sammenraste konstruksjoner som stillas og broer.<br />- brann – Alle branner utenom skog-/gress-/markbrann.<br />- brannABA – Automatisk brannalarm (ABA). Alarm fra bygg med direkte tilknytning til 110 sentralen.<br />- CBRNE – Fellesbetegnelse på hendelser som omfatter kjemiske stoffer (C), biologiske agens (B), radioaktive stoffer (R), nukleært materiale (N) og eksplosiver (E) med høyt farepotensiale.).<br />- personskade – Ulykker med personskade som ikke knyttes direkte til annen hendelsestype Merknad: personskade i forbindelse med annen definert hendelsestype skal angis som eget personobjekt i denne hendelsen. (F.eks. skadet personobjekt knyttet til skred, trafikkulykke eller brann).<br />- savnetPerson – En situasjon der en person ikke kan lokaliseres og antas å være i fare eller trenger assistanse.<br />- personIFare – Hendelser der personer er i fare uten at det nødvendigvis har oppstått skade. Inkluderer isolerte personer/grupper.<br />- sjøhendelse – Hendelse i sjø (vann, hav, mv.), slik som kollisjon mellom fartøy og fartøy i nød. Inkluderer "sjøhendelse" som definert i planverket for redningstjenesten.<br />- personIVann – Situasjon der en person i vann er i fare, inkludert person/mann over bord<br />- dykkerulykke – En ulykke som oppstår under dykking, inkludert trykkrelaterte skader, utstyrsfeil, eller andre hendelser som setter dykkerens liv og helse i fare.<br />- lufthendelse – En hendelse relatert til luftfart, inkludert ulykker med luftfartøy, nødsituasjoner i luften, eller fare for objekter på bakken. Inkluderer "lufthendelse" som definert i planverket for redningstjenesten.<br />- annenUlykke – Ulykke som ikke inngår i forhåndsdefinerte ulykkeskategorier.</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Hendelse

#### Hendelsesrelatert (abstrakt)

Informasjon som er direkte knyttet til hendelsen, men som ikke indikerer hendelsestype (se angitte verdier).

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kommentar</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Kort beskrivelse som fritekst.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>registreringstidspunkt</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Dato og tid for registrering av hendelsesrelatert informasjon.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>DateTime</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Felles

#### Objekt

Objekter på hendelsesstedet, samt observerte forhold ( objekter eller fenomenrer)  knyttet til hendelsen.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>typeObjekt</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Objekter fra kodelisten "TypeObjekt".</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeObject</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- nødsignal – Ethvert signal som brukes til å påkalle oppmerksomhet ifm nødssituasjon og ved andre omstendigheter hvor oppmerksomhet er krevet.<br />- spor – Klesplagg, mobil o.l. som kan knyttes til (er relevant for) et søk etter savnet person.<br />- funn – Funn av savnet person.<br />- person – Person (inkludert skadde på hendelsesstedet).<br />- last – Eks. gods fra varebil eller jernbanevogn som er spredt utover hendelsesområdet ved en ulykke.<br />- transportmiddel – Transportmiddel som er observert i tilknyting til hendelsen.<br />- bygg – Bygg som er relevant for håndtering av hendelsen.<br />- dyr – Dyr<br />- annet – Objekter som ikke inngår i de forhåndsdefinerte typene.<br />- ikkeSatt – Verdien er ikke lagt inn.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Dette er posisjonen til objektet. Dersom det er flere observasjoner kan også posisjonen estimeres basert på disse observasjonene. Det kan også være at enkelte observasjoner har større troverdighet enn andre og dermed bør vektes mer.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Object</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjonskvalitet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Beskriver usikkerhet knyttet til posisjonen. Det kan være en eksakt posisjon, men det kan også være knyttet usikkerhet til hvor objektet er innenfor et større eller mindre område. Dette angis med et valgt eksempelområde fra kodelisten "Posisjonskvalitet".</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Posisjonskvalitet</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- eksakt – Eks: gps-posisjon, veikryss, hushjørne.<br />- eiendomAdresseKjentPunkt – Lokasjon kan knyttes til eiendom, adresse eller kjent fast punkt (som tjern eller topp)<br />- nabolagKvartal – Lokasjon kan knyttes til nabolag/kvartal, eller tilsvarende areal.<br />- byTettsted – By/tettsted eller tilsvarende areal<br />- kommune – Lokasjon er knyttet til kommune<br />- ikkeSatt – Verdien er ikke lagt inn.</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Hendelsesrelatert

**Assosiasjoner**
Hendelse
Tiltakslokasjon
Observasjon – rolle: observasjon – kardinalitet: 1..*

#### Observasjon

Registrerte iakttakelser/fenomener som er relevante for hendelsen.<br />Merknad: Observasjoner er knyttet til objekt, jf.  kodeliste for objekttyper.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>observasjonsmåte</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Angir hvordan man har observert.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Observasjonsmåte</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- sett – Observsjonen er sett av noen.<br />- berørt – Observasjonen er gjort ved berøring.<br />- hørt – observasjon er gjort ved hørsel.<br />- luktet – observasjon er gjort ved lukt.<br />- annet – Objekter som ikke inngår i de forhåndsdefinerte typene.<br />- ikkeSatt – Verdien er ikke lagt inn.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>observasjonskvalitet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Informasjonens pålitelighet og nøyaktighet (som ikke gjelder posisjonskvalitet).</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Observasjonskvalitet</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- høy – Høy kvalitet<br />- middels – Middels kvalitet<br />- lav – Lav kvalitet<br />- ikkeSatt</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>observasjonFraTid</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>starttidspunkt for observasjonen.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>DateTime</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>observasjonTilTid</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>sluttidspunkt for observasjonen.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>DateTime</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>objektPosisjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>den angitte posisjonen til objektet, angitt fra observatør.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Objekt</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>observertFraPosisjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Hvor observasjonen ble observert fra. Dette kan være et eksakt punkt, men det kan også bli angitt som for eksempel en veistrekning eller et område.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Object</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjonskvalitet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Dette er en grov angivelse av hvor presist man har angitt posisjonen til objektet, basert på utsrekningen av et utvalg av områder. Dersom man vet at observasjonen er gjort i en liten skog, kan man velge å angi posisjonskvaliteten til "nabolagKvartal". Dersom man bare får opplyst at observasjonen er gjort i en bestemt stor skog, kan man benytte verdien "byTettsted".</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Posisjonskvalitet</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- eksakt – Eks: gps-posisjon, veikryss, hushjørne.<br />- eiendomAdresseKjentPunkt – Lokasjon kan knyttes til eiendom, adresse eller kjent fast punkt (som tjern eller topp)<br />- nabolagKvartal – Lokasjon kan knyttes til nabolag/kvartal, eller tilsvarende areal.<br />- byTettsted – By/tettsted eller tilsvarende areal<br />- kommune – Lokasjon er knyttet til kommune<br />- ikkeSatt – Verdien er ikke lagt inn.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>observatør</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Person eller sensor som gjør en observasjon.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Observatør</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>observatør.kontaktinformasjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Kontaktinformasjon</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterStreng</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>observatør.OPSoperatør</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Angir om operatøren er tilknyttet OPS.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>observatør.sensor</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>om observasjonen er gjort fra en automatisk sensor.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Hendelsesrelatert

**Assosiasjoner**
Objekt – rolle: objekt – kardinalitet: 1..*
Observatør – rolle: observatør – kardinalitet: 1

#### Ressurs (abstrakt)

Transportmiddel, personell, utstyr, materiell, etc. som kan mobiliseres for å støtte innsats og håndtering av en hendelse.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Angir ressursens posisjon (statisk/dynamisk) til enhver tid, innhentet fra relevant tjeneste.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Punkt</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>aktør</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Aktører fra kodelsisten "Aktør". I hovedsak nød- og beredskapsetater.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Aktør</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- politi – Politi<br />- helse – Helse<br />- brann – Brann<br />- HRS<br />- forsvar – Forsvar<br />- sivilforsvar – Sivilforsvar<br />- industrivern – Industriens egen beredskap som raskt kan håndtere hendelser før nødetatene kommer.<br />- frivilligeOrganisasjoner – Frivillige organisasjoner som har en rolle i håndteringen av en hendelse (inkluderer blant annet Røde Kors Hjelpekorps, Norsk Folkehjelp Sanitet, Redningsselskapet, Norske Redningshunder, Norsk Radio Relæ Liga, Speidernes Beredskapsgrupper, Norsk Grotteforbund, NLFs Flytjeneste).<br />- offentligeAktører – Inkluderer statlige og kommunale virksomheter (f.eks. statsforvalter, kommunens krisestab).<br />- andreAktører – Inkluderer relevant ekspertise (som ikke knyttes til bestemt virksomhet) eller andre som bidrar i eller får en rolle i hendelsen (f.eks. privatpersoner).</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>ressursID</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Aktørenes ID/kallesignal på egne ressurser.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>estimertAnkomsttid</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Når ressursen forventes å kunne være på hendelsesstedet.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>DateTime</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>tilgjengelighetOps</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Angir tilgjengeligheten av ressurser sett fra operasjonssentralens perspektiv, inkludert både operative og potensielt tilgjengelige ressurser.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TilgjengelighetOps</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- opptatt – Ressurs er tildelt hendelse.<br />- delvisTilgjengelig – Ressurs kan tildeles hendelse på kort varsel.<br />- ledig – Ressurs kan tildeles hendelse umiddelbart.<br />- ikkeSatt – Tilgjengelighet ikke angitt.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>tilgjengelighetHendelse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Angir tilgjengeligheten av ressurser som er tilordnet en pågående hendelse.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TilgjengelighetHendelse</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- opptatt – Ressurs er i aktiv innsats i hendelsen.<br />- delvisTilgjengelig – Ressurs er i aktiv innsats, men kan tildeles andre oppgaver på kort varsel.<br />- ledig – Ressurs er tilgjengelig for nye tiltak i hendelsen.<br />- ikkeSatt – Tilgjengelighet ikke angitt.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kommentar</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Mulighet for å legge inn kommentar som fritekst.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>status</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Felles

**Assosiasjoner**
Hendelse – rolle: hendelse – kardinalitet: 0..1
Tiltakslokasjon – kardinalitet: 0..*

#### Drone

Et ubemannet fartøy som kan operere i luft, på land, og/eller til vanns, enten autonomt eller fjernstyrt.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>synsfelt</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Flate</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>dronetype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Dronetyper</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeDrone</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- droneLuft – Ubemannede luftfartøy som kan operere autonomt eller fjernstyres, kjent som Unmanned Aerial Vehicles (UAV).<br />- droneVann – Ubemannede systemer designet for bruk på eller under vann som kan operere autonomt eller fjernstyres, ofte kalt maritime droner eller Unmanned Underwater Vehicles (UUV).<br />- droneLand – Ubemannede bakkebaserte kjøretøy som kan operere autonomt eller fjernstyres, også kalt Unmanned Ground Vehicles (UGV).<br />- droneAnnen – Droner som kombinerer egenskaper fra ulike miljøer, designet for å operere både til vanns og til lands – og eventuelt også i lufta. Disse omtales ofte som amfibiedroner eller flerbruksdroner.</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Ressurs

**Assosiasjoner**
Personell – rolle: droneoperatør – kardinalitet: 0..1

#### Depot

Et lager eller oppbevaringssted for utstyr, forsyninger eller ressurser, ofte strategisk plassert for å støtte operasjoner og sikre rask tilgang under nødsituasjoner eller beredskap.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>utstyr</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeUtstyr</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Ressurs

#### AnnenRessurs

Andre ikke kategoriserte ressurser.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>type</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Andre ikke kategoriserte ressurser. Restkategoriene er listet opp i "TypeAnnenRessurs".</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeAnnenRessurs</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- hund – Inkluderer politihund, redningshund mv.<br />- aggregat – Strømagregat<br />- annenRessurs – Annen ressurs inkluderer også utstyr som ikke kan knyttes til Transportmiddel eller Personell.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>utstyr</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Utstyr</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeUtstyr</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Ressurs

#### Transportmiddel

Inkluderer alle transportmidler definert under ressurstypen.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>type</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Kategorier av transportmiddel.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeTransportmiddel</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- litenBil – Personbil/stasjonsvogn – slik som legebil, innsatslederbil og kommandobil.<br />- storBil – Inkluderer ambulanse, mannskapsbil, dykkerbil, høyderedskap, tankbil, dronebil mv.<br />- båt – Inkluderer ambulanse/legebåt, brannbåt, politibåt, RS-båt, mv.<br />- helikopterUtenLift – Helikopter<br />- helikopterMedLift – Helikopter<br />- fly – Fly<br />- tog – Tog<br />- snøscooter – Snøscooter<br />- vannscooter – Vannscooter<br />- hest – Hest<br />- motorsykkel – Motorsykkel<br />- sykkel – Sykkel<br />- buss – Buss<br />- annetTransportmiddel – Transportmiddel som ikke inngår i forhåndsdefinerte transportmiddelkategorier.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>rolle</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeRolle</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- innsatsleder – Nødetatenes øverste leder på hendelsesstedet.<br />- delleder – Person med ansvar for ledelse av deloppgaver under hendelsen (f.eks. medisinsk leder, ressurskoordinator, fagleder innen spesifikke områder mv.).<br />- lege – Lege</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>utstyr</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeUtstyr</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Ressurs

#### Personell

Inkluderer alt personell definert under ressurstypen.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>rolle</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Personellroller</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeRolle</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- innsatsleder – Nødetatenes øverste leder på hendelsesstedet.<br />- delleder – Person med ansvar for ledelse av deloppgaver under hendelsen (f.eks. medisinsk leder, ressurskoordinator, fagleder innen spesifikke områder mv.).<br />- lege – Lege</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>typeEkspert</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Person med spesialistkompetanse som er tildelt en rådgivende rolle ifm. håndteringen av en hendelse.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeEkspert</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- CBRNE – Ekspertise innen kjemiske, biologiske, radiologiske, nukleære og eksplosive trusler, inkludert helserelevant ekspertise for å håndtere og respondere på farer knyttet til farlige stoffer og eksplosiver.<br />- geotekniskRiskoOgNaturfare – Ekspertise innen jordstabilitet, grunnforhold, skred, seismisk risiko mv.<br />- flom – Ekspertise innen flom, flomutsatte områder, flomdynamikk og tiltak mot flomfare.<br />- brannSkogbrann – Ekspertise innen brannslukking, spredning, evakuering mv.<br />- værKlimarisiko – Ekspertise innen værforhold, klimarisiko, og ekstreme værhendelser, inkludert hvordan klimaendringer påvirker hendelser som flom, tørke og stormer.<br />- sjøKystfare – Ekspertise innen kyst- og sjørelaterte hendelser, som stormflo, kysterosjon og maritime ulykker.<br />- epidemiologiSmittevern – Ekspertise innen smitte og sykdomsutbrudd, inkludert responstiltak.<br />- transportInfrastruktursikkerhet – Ekspertise innen transportnettverk og kritisk infrastruktur, som veier, jernbane, kraftnett mv.<br />- søkRedning – Ekspertise innen søk- og redningsoperasjoner, inkludert USAR.<br />- annenEkspertise – Ekspertise innen områder som ikke dekkes av de andre kategoriene.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>utstyr</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Utstyr</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeUtstyr</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Ressurs

**Assosiasjoner**
Transportmiddel – rolle: transportmiddel – kardinalitet: 0..1

#### Tiltakslokasjon

Lokasjon til tiltak som planlegges og eventuelt gjennomføres for å håndtere hendelsen.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Geometri (punkt/linje/flate) knyttet til tiltak.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>type</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Kode fra en kodeliste med relevante tiltak.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeTiltakslokasjon</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- oppmøtested – Et forhåndsdefinert sted hvor innsatspersonell først møter.<br />- bevarÅsted – "Bevar åsted" innebærer at ingen skal røre noe uten at nødvendig dokumentasjon av omstendighetene er foretatt og sikring av spor er gjennomført, med mindre det er nødvendig for å redde liv, pågripe eller berge større verdier.<br />- møtepunkt – Punkt der nødetatene har avtalt å møtes. Inkluderer situasjoner der samhandling mellom ulike ressurser er nødvendig.<br />- leveringssted – Behandlingssted for levering av pasienter.<br />- kontrollpunkt – Bemannet punkt for ulike typer kontroll, inkludert kontroll av tilgang til avgrensede områder, registrering av personer som evakueres (evakueringspunkt) etc.<br />- kommandoplass<br />- innsatsledersKO – Stedet hvor innsatslederne fra brann, politi og helse samles for å lede og koordinere innsatsen under en hendelse. Dette fungerer som et taktisk knutepunkt for informasjonsutveksling og beslutningstaking. (IL-KO).<br />- helsehjelp – Et dedikert område på eller nær et skadested hvor medisinsk behandling gis til skadde eller syke personer. Kan inkludere fasiliteter for førstehjelp og mer omfattende medisinsk hjelp.<br />- triage – Arbeidsprosess med hensikt å bestemme prioritering til behandling og transport basert på hvor alvorlig pasientenes medisinske tilstand er (Helsedirektoratet)<br />- dekontaminering – Dekontaminasjon: fjerning av forurensninger (kontaminasjoner) som har spredt seg innen et begrenset område. Slike forurensninger kan finnes på faste overflater av ulik type, i væsker eller i gasser. De kan bestå av giftige eller miljøresistente kjemikalier, mikroorganismer (bakterier o.l.) og av radioaktive substanser (SNL).<br />- samleplass – Inkluderer sampleplass for døde, skadde, uskadde, vitner, berørte etc.<br />- mottakssenter – Sted hvor man mottar et større antall evakuerte og/ eller skadde fra en hendelse på sjøen eller i utlandet. Mottakssenteret kan også benyttes som en samleplass for evakuerte eller skadde eller som et evakueringspunkt dersom det er hensiktsmessig (PBS 1).<br />- evakuerteOgPårørendesenter – Oppholdssted for evakuerte som ikke er skadet, samt oppmøtested for pårørende.<br />- presseOgMedia – Et dedikert område for håndtering av mediekontakt under hendelser eller operasjoner, hvor journalister kan få informasjon.<br />- observasjonspost – En strategisk plassert posisjon for overvåking og innsamling av informasjon om et bestemt område, ofte brukt til å identifisere risiko, observere hendelser eller koordinere respons.<br />- helikopterlandingsplass – Et tilrettelagt område for trygg landing og avgang av helikoptre, ofte brukt i redningsarbeid, beredskap eller transport til vanskelig tilgjengelige steder.<br />- sambandsinstallasjon – En teknisk installasjon som muliggjør kommunikasjon og informasjonsdeling, ofte brukt i nødetatens og beredskapsaktørers arbeid for å sikre effektiv koordinering.<br />- depot – Lager (opprettet for håndtering av hendelsen) der det oppbevares større mengder materiell for senere bruk.<br />- parkeringsplass – Parkeringsplass<br />- kjørerute – Angivelse av definert kjørerute fra ressursens lokasjon til hendelsessted. Innhentet fra relevant tjeneste.<br />- sikkerRute – Sikker rute for nødetatene inn og ut fra hendelsessted (inkl. for helsepersonell som skal inn til skadde personer, samt evakueringslinje/akse, jf. Håndbok for redningstjeneste). Inkluderer sikker innpå marsj (polititerminologi.).<br />- avsperring – Sperringstiltak oppsatt ifm. en hendelse som marker definerte områder hvor kun nødetater og annet autorisert personell kan oppholde seg. Avsperring settes i kartet iht. etablerte prosedyrer for nødetatene.<br />- evakueringssone – Sone som personer skal evakueres fra.<br />- søketeigsone – Definert område hvor det søkes etter savnede. Merkes iht gjeldende regler for søkeoppdrag (Se Nasjonal veileder søk etter savnet person på land (2022)).<br />- faresone – Definerte områder rundt hendelsen som indikerer grad av risiko for de som oppholder seg der.<br />- sikring – Forebyggende tiltak i forbindelse med brann, flom, utslipp etc.<br />- arbeidsområde – Område som avgrenses for nødetatenes særskilte tiltak under håndteringen av hendelsen.<br />- slukking – Prosessen med å bekjempe og eliminere brann ved hjelp av ulike metoder og utstyr for å stoppe brannens spredning og redusere skadeomfanget.<br />- vannbombing – En metode for brannslukking hvor store mengder vann slippes fra fly eller helikoptre over brannområder, spesielt effektivt ved skogbranner.<br />- begrensningslinjeVåt – En fysisk eller strategisk linje etablert for å hindre videre spredning av brann, ofte ved bruk av naturlige barrierer eller opprettede brannlinjer (Bruk av vann).<br />- begrensningslinjeTørr – En fysisk eller strategisk linje etablert for å hindre videre spredning av brann, ofte ved bruk av naturlige barrierer eller opprettede brannlinjer (uten bruk av vann).<br />- vannslange – Slange brukt i brannslukking for å transportere og levere vann til brannstedet.<br />- vannpumpe – Pumpe brukt i brannslukking for å transportere og levere vann til brannstedet.<br />- sektorgrense – En definert avgrensning mellom ulike sektorer på et skadested, som brukes for å organisere og koordinere innsatsen effektivt.<br />- referansesystem – System som brukes for å identifisere og beskrive spesifikke steder innenfor et område. Brukes ofte for koordinering, spesielt i nødsituasjoner eller komplekse omgivelser.<br />- annetTiltak – Ikke forhåndsdefinerte tiltak</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>aktør</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Aktører fra kodelsisten "Aktør". I hovedsak nød- og beredskapsetater.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Aktør</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- politi – Politi<br />- helse – Helse<br />- brann – Brann<br />- HRS<br />- forsvar – Forsvar<br />- sivilforsvar – Sivilforsvar<br />- industrivern – Industriens egen beredskap som raskt kan håndtere hendelser før nødetatene kommer.<br />- frivilligeOrganisasjoner – Frivillige organisasjoner som har en rolle i håndteringen av en hendelse (inkluderer blant annet Røde Kors Hjelpekorps, Norsk Folkehjelp Sanitet, Redningsselskapet, Norske Redningshunder, Norsk Radio Relæ Liga, Speidernes Beredskapsgrupper, Norsk Grotteforbund, NLFs Flytjeneste).<br />- offentligeAktører – Inkluderer statlige og kommunale virksomheter (f.eks. statsforvalter, kommunens krisestab).<br />- andreAktører – Inkluderer relevant ekspertise (som ikke knyttes til bestemt virksomhet) eller andre som bidrar i eller får en rolle i hendelsen (f.eks. privatpersoner).</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>status</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>En beskrivelse av tilstanden for fremdrift i tiltaket.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Status</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- planlagt – Tiltaket er planlagt.<br />- pågåendeEllerAktivt – Tiltaket er pågående eller aktivt.<br />- gjennomførtEllerAvsluttet – Tiltaket er gjennomført eller avsluttet.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>prioritetTilak</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Prioritet indikerer den enkelte etats planlagte rekkefølge på tiltak.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>typeFaresone</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeFaresone</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- rødSone – Område med høy risiko for liv/helse.<br />- gulSone – Område med risiko for liv/helse.<br />- grønnSone – Område med lav risiko for liv/helse.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>typeRute</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeRute</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- enveis – Man kan bare kjøre i en retning.<br />- toveis – Man kan bare kjøre i begge retninger.<br />- ikkeSatt – Kjøreretning er ikke satt.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>bevarÅsted</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>"Bevar åsted" innebærer at ingen skal røre noe uten at nødvendig dokumentasjon av omstendighetene er foretatt og sikring av spor er gjennomført, med mindre det er nødvendig for å redde liv, pågripe eller berge større verdier.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kommentar</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Mulighet for å legge inn kommentar som fritekst.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Felles

**Assosiasjoner**
Hendelse – rolle: hendelse
Objekt – rolle: lokasjon – kardinalitet: 0..1
Ressurs
X___TiltakOppgave

#### Kontekst

Informasjon som i utgangspunktet ikke er knyttet til hendelsen, men som det er viktig/relevant for nødetatene å kjenne til fordi det potensielt kan eller bør påvirke beslutninger om tiltak/håndtering.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>type</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>En kategorisering av ulik type kontekst.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeKontekst</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- farekilder – Identifisert kilde som kan utgjøre en fare for spredning av risiko under håndteringen av en hendelse, f. eks. eksplosiver, radioaktiv agens etc.<br />- beskyttelsesverdigInfrastruktur – Identifisert infrastruktur som kan utsettes for økt risiko som følge av hendelsen.<br />- sårbartObjekt – Objekter som kan være spesielt sårbare som følge av hendelsen, slik som skoler, barnehager, sykehjem, kulturminner etc.<br />- ødelagtInfrastruktur – Ødelagt infrastruktur som aktørene i hendelsen bør vite om.<br />- folkeansamling – Konsentrasjon av mennesker, f.eks. knyttet til uteliv, arrangementer o.l.<br />- hinderSperring – Fysisk hindring/sperring som kan påvirke fremkommeligheten under en hendelse uten å være en del av selve hendelsen, f.eks. veltede trær, veisperringer eller ødelagte broer som hindrer transport og evakuering.<br />- spenningsløsKraftledning – Kraftledning som er frakoblet strømnettet og dermed ikke lenger utgjør fare for elektrisk støt. Brukes som varsel i hendelseshåndtering for å informere om at det er trygt å bevege seg i nærheten eller under ledningen, for eksempel ved en togulykke.<br />- annenKontekst – Kontekstuell informasjon som ikke inngår i forhåndsdefinerte kategorier.</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>aktør</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Aktører fra kodelsisten "Aktør", som er relevant for kontekstregistreringen.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Aktør</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- politi – Politi<br />- helse – Helse<br />- brann – Brann<br />- HRS<br />- forsvar – Forsvar<br />- sivilforsvar – Sivilforsvar<br />- industrivern – Industriens egen beredskap som raskt kan håndtere hendelser før nødetatene kommer.<br />- frivilligeOrganisasjoner – Frivillige organisasjoner som har en rolle i håndteringen av en hendelse (inkluderer blant annet Røde Kors Hjelpekorps, Norsk Folkehjelp Sanitet, Redningsselskapet, Norske Redningshunder, Norsk Radio Relæ Liga, Speidernes Beredskapsgrupper, Norsk Grotteforbund, NLFs Flytjeneste).<br />- offentligeAktører – Inkluderer statlige og kommunale virksomheter (f.eks. statsforvalter, kommunens krisestab).<br />- andreAktører – Inkluderer relevant ekspertise (som ikke knyttes til bestemt virksomhet) eller andre som bidrar i eller får en rolle i hendelsen (f.eks. privatpersoner).</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kommentar</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Mulighet for å legge inn kommentar som fritekst.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Posisjon</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjon.geometri</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Object</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjon.Referanse</strong></td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Identifikasjon</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjon.Referanse.lokalId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>lokal identifikator av et objekt<br /><br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>uuid</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjon.Referanse.navnerom</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br /><br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br /><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjon.Referanse.versjonId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Felles

**Assosiasjoner**
Hendelse – rolle: hendelse

### Kodelister

#### «Enumeration» TypeHelsesamvirke

**Definisjon:** Kategorier av hendelsestypen helsesamvikre

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>firstResponder</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>tvang</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Hovedaktør

**Definisjon:** enhet som bidrar i å håndtere en hendelse, begrenset til politi, brann, helse eller HRS.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>politi</td>
      <td>Politi</td>
      <td></td>
    </tr>
    <tr>
      <td>helse</td>
      <td>Helse</td>
      <td></td>
    </tr>
    <tr>
      <td>brann</td>
      <td>Brann</td>
      <td></td>
    </tr>
    <tr>
      <td>HRS</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» PrioritetHendelse

**Definisjon:** Hendelse som krever umiddelbar respons (akutt)

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>høy</td>
      <td>Hendelse som krever umiddelbar respons (akutt)</td>
      <td></td>
    </tr>
    <tr>
      <td>middels</td>
      <td>Hendelse som krever rask respons</td>
      <td></td>
    </tr>
    <tr>
      <td>lav</td>
      <td>Hendelse som krever respons</td>
      <td></td>
    </tr>
    <tr>
      <td>ingen</td>
      <td>ingenPrioritet</td>
      <td></td>
    </tr>
    <tr>
      <td>ikkeSatt</td>
      <td>Prioritet ikke vurdert</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Kompleksitet

**Definisjon:** Et uttrykk for hvor krevende/komplisert det er å håndtere en hendelse

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>komplisert</td>
      <td>Hendelser som er særlig utfordrende å håndtere, eksempelvis på grunn av sitt omfang, krav til spesialisert kompetanse, tilgjengelighet til hendelsessted og/eller krav til koordinering mellom nødetatene.</td>
      <td></td>
    </tr>
    <tr>
      <td>rutine</td>
      <td>Hendelser som ikke defineres som komplekse</td>
      <td></td>
    </tr>
    <tr>
      <td>ikkeSatt</td>
      <td>Hendelsens kompleksitet ikke vurdert</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Lokalitetstype

**Definisjon:** Kjennetegn ved det stedet der hendelsen finner sted og som kan ha betydning for håndteringen. En gitt lokalitetstype kan inngå i en strukturert kategorisering av kjennetegn knyttet til blant annet naturforhold (som skog, sjø, fjell mv.), bebyggelse, befolkningstetthet og tilgjengelighet.

#### «Enumeration» TypePlanlagtHendelse

**Definisjon:** Kategorier av hendelsestypen planlagt hendelse.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>arrangement</td>
      <td>Planlagte arrangementer, f. eks idrett, kultur, konserter, festivaler ol.</td>
      <td></td>
    </tr>
    <tr>
      <td>demonstrasjon</td>
      <td>Planlagte demonstrasjoner.</td>
      <td></td>
    </tr>
    <tr>
      <td>VIP</td>
      <td>Planlagte hendelser som krever særskilt beskyttelse av deltakere i hendelsen, eksempelvis grunnet deres offisielle status som myndighetspersoner.</td>
      <td></td>
    </tr>
    <tr>
      <td>annenPlanlagtHendelse</td>
      <td>Planlagt hendelse som ikke inngår i de forhåndsdefinerte kategoriene for slike hendelser.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeUtbredelse

**Definisjon:** Spredningsbeskrivelser for et utvalg av hendelser som har begreper for utbredelse.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>hendelsesområde</td>
      <td>En generisk betegnelse for ustrekning av en hendelse som kan brukes dersom hendelsen ikke har begreper for områder som er rammet.</td>
      <td></td>
    </tr>
    <tr>
      <td>brannfront</td>
      <td>Den fremste delen av en brann hvor forbrenningen er mest intens og hvordan brannen sprer seg videre (retning, hastighet, tid, prognose, etc.).</td>
      <td></td>
    </tr>
    <tr>
      <td>aktivtBrannområde</td>
      <td>Området som er rammet av brannen, hvor det pågår aktiv brann.</td>
      <td></td>
    </tr>
    <tr>
      <td>brentOmråde</td>
      <td>Området som er rammet av brannen, som er brent.</td>
      <td></td>
    </tr>
    <tr>
      <td>skredområde</td>
      <td>Området som er rammet av skredet.</td>
      <td></td>
    </tr>
    <tr>
      <td>flomområde</td>
      <td>Området som er rammet av flommen.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeSikkerhetshendelse

**Definisjon:** Kategorier av hendelsestypen sikkerhetshendelse.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>vold</td>
      <td>En hendelse der fysisk makt, trusler eller overgrep utøves mot en eller flere personer, med potensial for skade på liv og helse.</td>
      <td></td>
    </tr>
    <tr>
      <td>orden</td>
      <td>En hendelse som krever tiltak for å gjenopprette eller opprettholde offentlig ro og sikkerhet, ofte relatert til forstyrrelser, uro eller situasjoner som kan eskalere til vold eller skade.</td>
      <td></td>
    </tr>
    <tr>
      <td>PLIVO</td>
      <td>En pågående situasjon der en eller flere gjerningspersoner utøver, eller er i ferd med å utøve, livstruende vold mot flere uskyldige personer. Skadeomfanget er, eller vurderes å kunne bli, så stort at nødetatene raskest mulig må gå i ekstraordinær innsats sammen, for å stanse handlingene og redde liv (Nasjonal prosedyre – PLIVO).</td>
      <td></td>
    </tr>
    <tr>
      <td>terror</td>
      <td>Terrorhandling: Ulovlig bruk av, eller trussel om bruk av, makt eller vold mot personer eller eiendom, i et forsøk på å legge press på landets myndigheter eller befolkning eller samfunnet for øvrig for å oppnå politiske, religiøse eller ideologiske mål (NOU 2016: 19 Samhandling for sikkerhet).</td>
      <td></td>
    </tr>
    <tr>
      <td>sabotasje</td>
      <td>Sabotasje er å skade eiendom, produksjonsmidler eller tekniske systemer med hensikt (SNL).</td>
      <td></td>
    </tr>
    <tr>
      <td>bombetrussel</td>
      <td>En hendelse der det blir fremsatt en påstand eller mistanke om at en eksplosiv enhet er plassert, noe som utløser behov for evakuering, søk og vurdering av risiko.</td>
      <td></td>
    </tr>
    <tr>
      <td>helserelatertSikkerhetssituasjon</td>
      <td>Hendelser som involverer personer som kan utgjøre en fare for seg selv eller andre, eksempelvis knyttet til rus eller psykisk tilstand.</td>
      <td></td>
    </tr>
    <tr>
      <td>annenSikkerhetshendelse</td>
      <td>Sikkerhetshendelse som ikke inngår i de forhåndsdefinerte typene.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeNaturhendelse

**Definisjon:** Kategorier av hendelsestypen naturhendelse.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>skred</td>
      <td>Masse (stein, løsmasser, leire, jord) som beveger seg nedover skråninger og/eller under vann (delvis basert på NVE m fl).</td>
      <td></td>
    </tr>
    <tr>
      <td>snøskred</td>
      <td>Masse (snø, våt eller tørr) som beveger seg raskt nedover en skråning (NVE m fl).</td>
      <td></td>
    </tr>
    <tr>
      <td>flom</td>
      <td>Vannføring som går ut over normale nivåer og som fører eller kan føre til skade på infrastruktur og/eller bebyggelse.</td>
      <td></td>
    </tr>
    <tr>
      <td>skogGressMarkbrann</td>
      <td>En brann som oppstår i vegetasjonsområder i innmark og utmark.</td>
      <td></td>
    </tr>
    <tr>
      <td>ekstremvær</td>
      <td>Vær som medfører fare for liv og verdier. Ekstremvær kan være sterk vind, kraftig nedbør, stormflo og høye bølger eller en kombinasjon av værelementer som til sammen utgjør en fare.</td>
      <td></td>
    </tr>
    <tr>
      <td>annenNaturhendelse</td>
      <td>Naturhendelse som ikke inngår i forhåndsdefinerte naturhendelsestyper.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeUlykke

**Definisjon:** Kategorier av hendelsestypen ulykke.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>trafikkulykke</td>
      <td>Ulykker som skjer på veiene i forbindelse med forflytting av mennesker og gods. Det kan være møteulykker, utforkjøringer og skader på fotgjengere og syklister (SNL).</td>
      <td></td>
    </tr>
    <tr>
      <td>jernbaneulykke</td>
      <td>En uønsket eller utilsiktet plutselig begivenhet eller en bestemt rekke slike begivenheter som har skadelige følger, herunder som medfører at noen dør eller blir alvorlig skadet, som medfører betydelig skade på jernbanemateriell, på kjørevei, på eiendom utenfor jernbanen eller på miljø, og alle andre lignende ulykker (Jernbaneundersøkelsesloven § 5).</td>
      <td></td>
    </tr>
    <tr>
      <td>tunnelulykkeVei</td>
      <td>Veiulykke i tunnel.</td>
      <td></td>
    </tr>
    <tr>
      <td>tunnelulykkeJernbane</td>
      <td>Jernbaneulykke i tunnel (se jernbaneulykke).</td>
      <td></td>
    </tr>
    <tr>
      <td>tunnelbrannVei</td>
      <td>Brann i veitunnel.</td>
      <td></td>
    </tr>
    <tr>
      <td>tunnelbrannJernbane</td>
      <td>Brann i jernbanetunnel.</td>
      <td></td>
    </tr>
    <tr>
      <td>bygningsulykke</td>
      <td>En ulykke som involverer skade eller sammenbrudd av en bygning, inkludert sammenraste konstruksjoner som stillas og broer.</td>
      <td></td>
    </tr>
    <tr>
      <td>brann</td>
      <td>Alle branner utenom skog-/gress-/markbrann.</td>
      <td></td>
    </tr>
    <tr>
      <td>brannABA</td>
      <td>Automatisk brannalarm (ABA). Alarm fra bygg med direkte tilknytning til 110 sentralen.</td>
      <td></td>
    </tr>
    <tr>
      <td>CBRNE</td>
      <td>Fellesbetegnelse på hendelser som omfatter kjemiske stoffer (C), biologiske agens (B), radioaktive stoffer (R), nukleært materiale (N) og eksplosiver (E) med høyt farepotensiale.).</td>
      <td></td>
    </tr>
    <tr>
      <td>personskade</td>
      <td>Ulykker med personskade som ikke knyttes direkte til annen hendelsestype Merknad: personskade i forbindelse med annen definert hendelsestype skal angis som eget personobjekt i denne hendelsen. (F.eks. skadet personobjekt knyttet til skred, trafikkulykke eller brann).</td>
      <td></td>
    </tr>
    <tr>
      <td>savnetPerson</td>
      <td>En situasjon der en person ikke kan lokaliseres og antas å være i fare eller trenger assistanse.</td>
      <td></td>
    </tr>
    <tr>
      <td>personIFare</td>
      <td>Hendelser der personer er i fare uten at det nødvendigvis har oppstått skade. Inkluderer isolerte personer/grupper.</td>
      <td></td>
    </tr>
    <tr>
      <td>sjøhendelse</td>
      <td>Hendelse i sjø (vann, hav, mv.), slik som kollisjon mellom fartøy og fartøy i nød. Inkluderer "sjøhendelse" som definert i planverket for redningstjenesten.</td>
      <td></td>
    </tr>
    <tr>
      <td>personIVann</td>
      <td>Situasjon der en person i vann er i fare, inkludert person/mann over bord</td>
      <td></td>
    </tr>
    <tr>
      <td>dykkerulykke</td>
      <td>En ulykke som oppstår under dykking, inkludert trykkrelaterte skader, utstyrsfeil, eller andre hendelser som setter dykkerens liv og helse i fare.</td>
      <td></td>
    </tr>
    <tr>
      <td>lufthendelse</td>
      <td>En hendelse relatert til luftfart, inkludert ulykker med luftfartøy, nødsituasjoner i luften, eller fare for objekter på bakken. Inkluderer "lufthendelse" som definert i planverket for redningstjenesten.</td>
      <td></td>
    </tr>
    <tr>
      <td>annenUlykke</td>
      <td>Ulykke som ikke inngår i forhåndsdefinerte ulykkeskategorier.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeObject

**Definisjon:** Angir hva som er observert.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>nødsignal</td>
      <td>Ethvert signal som brukes til å påkalle oppmerksomhet ifm nødssituasjon og ved andre omstendigheter hvor oppmerksomhet er krevet.</td>
      <td></td>
    </tr>
    <tr>
      <td>spor</td>
      <td>Klesplagg, mobil o.l. som kan knyttes til (er relevant for) et søk etter savnet person.</td>
      <td></td>
    </tr>
    <tr>
      <td>funn</td>
      <td>Funn av savnet person.</td>
      <td></td>
    </tr>
    <tr>
      <td>person</td>
      <td>Person (inkludert skadde på hendelsesstedet).</td>
      <td></td>
    </tr>
    <tr>
      <td>last</td>
      <td>Eks. gods fra varebil eller jernbanevogn som er spredt utover hendelsesområdet ved en ulykke.</td>
      <td></td>
    </tr>
    <tr>
      <td>transportmiddel</td>
      <td>Transportmiddel som er observert i tilknyting til hendelsen.</td>
      <td></td>
    </tr>
    <tr>
      <td>bygg</td>
      <td>Bygg som er relevant for håndtering av hendelsen.</td>
      <td></td>
    </tr>
    <tr>
      <td>dyr</td>
      <td>Dyr</td>
      <td></td>
    </tr>
    <tr>
      <td>annet</td>
      <td>Objekter som ikke inngår i de forhåndsdefinerte typene.</td>
      <td></td>
    </tr>
    <tr>
      <td>ikkeSatt</td>
      <td>Verdien er ikke lagt inn.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Posisjonskvalitet

**Definisjon:** Beskrivelse av kvaliteten på stedfestingen. Angir grad av presisjon knyttet til posisjon.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>eksakt</td>
      <td>Eks: gps-posisjon, veikryss, hushjørne.</td>
      <td></td>
    </tr>
    <tr>
      <td>eiendomAdresseKjentPunkt</td>
      <td>Lokasjon kan knyttes til eiendom, adresse eller kjent fast punkt (som tjern eller topp)</td>
      <td></td>
    </tr>
    <tr>
      <td>nabolagKvartal</td>
      <td>Lokasjon kan knyttes til nabolag/kvartal, eller tilsvarende areal.</td>
      <td></td>
    </tr>
    <tr>
      <td>byTettsted</td>
      <td>By/tettsted eller tilsvarende areal</td>
      <td></td>
    </tr>
    <tr>
      <td>kommune</td>
      <td>Lokasjon er knyttet til kommune</td>
      <td></td>
    </tr>
    <tr>
      <td>ikkeSatt</td>
      <td>Verdien er ikke lagt inn.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Observasjonsmåte

**Definisjon:** Angir hvordan observasjonen er gjort av observatør: sett, hørt, berørt, luktet, annet, ikke satt.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>sett</td>
      <td>Observsjonen er sett av noen.</td>
      <td></td>
    </tr>
    <tr>
      <td>berørt</td>
      <td>Observasjonen er gjort ved berøring.</td>
      <td></td>
    </tr>
    <tr>
      <td>hørt</td>
      <td>observasjon er gjort ved hørsel.</td>
      <td></td>
    </tr>
    <tr>
      <td>luktet</td>
      <td>observasjon er gjort ved lukt.</td>
      <td></td>
    </tr>
    <tr>
      <td>annet</td>
      <td>Objekter som ikke inngår i de forhåndsdefinerte typene.</td>
      <td></td>
    </tr>
    <tr>
      <td>ikkeSatt</td>
      <td>Verdien er ikke lagt inn.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Observasjonskvalitet

**Definisjon:** Informasjonens pålitelighet og nøyaktighet (som ikke gjelder posisjonskvalitet).

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>høy</td>
      <td>Høy kvalitet</td>
      <td></td>
    </tr>
    <tr>
      <td>middels</td>
      <td>Middels kvalitet</td>
      <td></td>
    </tr>
    <tr>
      <td>lav</td>
      <td>Lav kvalitet</td>
      <td></td>
    </tr>
    <tr>
      <td>ikkeSatt</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Aktør

**Definisjon:** En kodelsiste med aktører. I hovedsak nød- og beredskapsetater.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>politi</td>
      <td>Politi</td>
      <td></td>
    </tr>
    <tr>
      <td>helse</td>
      <td>Helse</td>
      <td></td>
    </tr>
    <tr>
      <td>brann</td>
      <td>Brann</td>
      <td></td>
    </tr>
    <tr>
      <td>HRS</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>forsvar</td>
      <td>Forsvar</td>
      <td></td>
    </tr>
    <tr>
      <td>sivilforsvar</td>
      <td>Sivilforsvar</td>
      <td></td>
    </tr>
    <tr>
      <td>industrivern</td>
      <td>Industriens egen beredskap som raskt kan håndtere hendelser før nødetatene kommer.</td>
      <td></td>
    </tr>
    <tr>
      <td>frivilligeOrganisasjoner</td>
      <td>Frivillige organisasjoner som har en rolle i håndteringen av en hendelse (inkluderer blant annet Røde Kors Hjelpekorps, Norsk Folkehjelp Sanitet, Redningsselskapet, Norske Redningshunder, Norsk Radio Relæ Liga, Speidernes Beredskapsgrupper, Norsk Grotteforbund, NLFs Flytjeneste).</td>
      <td></td>
    </tr>
    <tr>
      <td>offentligeAktører</td>
      <td>Inkluderer statlige og kommunale virksomheter (f.eks. statsforvalter, kommunens krisestab).</td>
      <td></td>
    </tr>
    <tr>
      <td>andreAktører</td>
      <td>Inkluderer relevant ekspertise (som ikke knyttes til bestemt virksomhet) eller andre som bidrar i eller får en rolle i hendelsen (f.eks. privatpersoner).</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TilgjengelighetOps

**Definisjon:** Angir tilgjengeligheten av ressurser sett fra operasjonssentralens perspektiv, inkludert både operative og potensielt tilgjengelige ressurser.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>opptatt</td>
      <td>Ressurs er tildelt hendelse.</td>
      <td></td>
    </tr>
    <tr>
      <td>delvisTilgjengelig</td>
      <td>Ressurs kan tildeles hendelse på kort varsel.</td>
      <td></td>
    </tr>
    <tr>
      <td>ledig</td>
      <td>Ressurs kan tildeles hendelse umiddelbart.</td>
      <td></td>
    </tr>
    <tr>
      <td>ikkeSatt</td>
      <td>Tilgjengelighet ikke angitt.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TilgjengelighetHendelse

**Definisjon:** Angir tilgjengeligheten av ressurser tilordnet hendelsen.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>opptatt</td>
      <td>Ressurs er i aktiv innsats i hendelsen.</td>
      <td></td>
    </tr>
    <tr>
      <td>delvisTilgjengelig</td>
      <td>Ressurs er i aktiv innsats, men kan tildeles andre oppgaver på kort varsel.</td>
      <td></td>
    </tr>
    <tr>
      <td>ledig</td>
      <td>Ressurs er tilgjengelig for nye tiltak i hendelsen.</td>
      <td></td>
    </tr>
    <tr>
      <td>ikkeSatt</td>
      <td>Tilgjengelighet ikke angitt.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeDrone

**Definisjon:** Kategorier av dronetyper.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>droneLuft</td>
      <td>Ubemannede luftfartøy som kan operere autonomt eller fjernstyres, kjent som Unmanned Aerial Vehicles (UAV).</td>
      <td></td>
    </tr>
    <tr>
      <td>droneVann</td>
      <td>Ubemannede systemer designet for bruk på eller under vann som kan operere autonomt eller fjernstyres, ofte kalt maritime droner eller Unmanned Underwater Vehicles (UUV).</td>
      <td></td>
    </tr>
    <tr>
      <td>droneLand</td>
      <td>Ubemannede bakkebaserte kjøretøy som kan operere autonomt eller fjernstyres, også kalt Unmanned Ground Vehicles (UGV).</td>
      <td></td>
    </tr>
    <tr>
      <td>droneAnnen</td>
      <td>Droner som kombinerer egenskaper fra ulike miljøer, designet for å operere både til vanns og til lands – og eventuelt også i lufta. Disse omtales ofte som amfibiedroner eller flerbruksdroner.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «CodeList» TypeUtstyr

**Definisjon:** Lister som defineres fra nødetatene. Dette er foreløpig utelatt fra standarden.

#### «Enumeration» TypeAnnenRessurs

**Definisjon:** Ressurs som ikke inngår i forhåndsdefinerte ressurskategorier.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>hund</td>
      <td>Inkluderer politihund, redningshund mv.</td>
      <td></td>
    </tr>
    <tr>
      <td>aggregat</td>
      <td>Strømagregat</td>
      <td></td>
    </tr>
    <tr>
      <td>annenRessurs</td>
      <td>Annen ressurs inkluderer også utstyr som ikke kan knyttes til Transportmiddel eller Personell.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeTransportmiddel

**Definisjon:** Kategorier av transportmiddel.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>litenBil</td>
      <td>Personbil/stasjonsvogn – slik som legebil, innsatslederbil og kommandobil.</td>
      <td></td>
    </tr>
    <tr>
      <td>storBil</td>
      <td>Inkluderer ambulanse, mannskapsbil, dykkerbil, høyderedskap, tankbil, dronebil mv.</td>
      <td></td>
    </tr>
    <tr>
      <td>båt</td>
      <td>Inkluderer ambulanse/legebåt, brannbåt, politibåt, RS-båt, mv.</td>
      <td></td>
    </tr>
    <tr>
      <td>helikopterUtenLift</td>
      <td>Helikopter</td>
      <td></td>
    </tr>
    <tr>
      <td>helikopterMedLift</td>
      <td>Helikopter</td>
      <td></td>
    </tr>
    <tr>
      <td>fly</td>
      <td>Fly</td>
      <td></td>
    </tr>
    <tr>
      <td>tog</td>
      <td>Tog</td>
      <td></td>
    </tr>
    <tr>
      <td>snøscooter</td>
      <td>Snøscooter</td>
      <td></td>
    </tr>
    <tr>
      <td>vannscooter</td>
      <td>Vannscooter</td>
      <td></td>
    </tr>
    <tr>
      <td>hest</td>
      <td>Hest</td>
      <td></td>
    </tr>
    <tr>
      <td>motorsykkel</td>
      <td>Motorsykkel</td>
      <td></td>
    </tr>
    <tr>
      <td>sykkel</td>
      <td>Sykkel</td>
      <td></td>
    </tr>
    <tr>
      <td>buss</td>
      <td>Buss</td>
      <td></td>
    </tr>
    <tr>
      <td>annetTransportmiddel</td>
      <td>Transportmiddel som ikke inngår i forhåndsdefinerte transportmiddelkategorier.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeRolle

**Definisjon:** Kategorier av roller.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>innsatsleder</td>
      <td>Nødetatenes øverste leder på hendelsesstedet.</td>
      <td></td>
    </tr>
    <tr>
      <td>delleder</td>
      <td>Person med ansvar for ledelse av deloppgaver under hendelsen (f.eks. medisinsk leder, ressurskoordinator, fagleder innen spesifikke områder mv.).</td>
      <td></td>
    </tr>
    <tr>
      <td>lege</td>
      <td>Lege</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeEkspert

**Definisjon:** Person med spesialistkompetanse som er tildelt en rådgivende rolle ifm. håndteringen av en hendelse.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>CBRNE</td>
      <td>Ekspertise innen kjemiske, biologiske, radiologiske, nukleære og eksplosive trusler, inkludert helserelevant ekspertise for å håndtere og respondere på farer knyttet til farlige stoffer og eksplosiver.</td>
      <td></td>
    </tr>
    <tr>
      <td>geotekniskRiskoOgNaturfare</td>
      <td>Ekspertise innen jordstabilitet, grunnforhold, skred, seismisk risiko mv.</td>
      <td></td>
    </tr>
    <tr>
      <td>flom</td>
      <td>Ekspertise innen flom, flomutsatte områder, flomdynamikk og tiltak mot flomfare.</td>
      <td></td>
    </tr>
    <tr>
      <td>brannSkogbrann</td>
      <td>Ekspertise innen brannslukking, spredning, evakuering mv.</td>
      <td></td>
    </tr>
    <tr>
      <td>værKlimarisiko</td>
      <td>Ekspertise innen værforhold, klimarisiko, og ekstreme værhendelser, inkludert hvordan klimaendringer påvirker hendelser som flom, tørke og stormer.</td>
      <td></td>
    </tr>
    <tr>
      <td>sjøKystfare</td>
      <td>Ekspertise innen kyst- og sjørelaterte hendelser, som stormflo, kysterosjon og maritime ulykker.</td>
      <td></td>
    </tr>
    <tr>
      <td>epidemiologiSmittevern</td>
      <td>Ekspertise innen smitte og sykdomsutbrudd, inkludert responstiltak.</td>
      <td></td>
    </tr>
    <tr>
      <td>transportInfrastruktursikkerhet</td>
      <td>Ekspertise innen transportnettverk og kritisk infrastruktur, som veier, jernbane, kraftnett mv.</td>
      <td></td>
    </tr>
    <tr>
      <td>søkRedning</td>
      <td>Ekspertise innen søk- og redningsoperasjoner, inkludert USAR.</td>
      <td></td>
    </tr>
    <tr>
      <td>annenEkspertise</td>
      <td>Ekspertise innen områder som ikke dekkes av de andre kategoriene.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeTiltakslokasjon

**Definisjon:** En kodeliste med relevante tiltak.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>oppmøtested</td>
      <td>Et forhåndsdefinert sted hvor innsatspersonell først møter.</td>
      <td></td>
    </tr>
    <tr>
      <td>bevarÅsted</td>
      <td>"Bevar åsted" innebærer at ingen skal røre noe uten at nødvendig dokumentasjon av omstendighetene er foretatt og sikring av spor er gjennomført, med mindre det er nødvendig for å redde liv, pågripe eller berge større verdier.</td>
      <td></td>
    </tr>
    <tr>
      <td>møtepunkt</td>
      <td>Punkt der nødetatene har avtalt å møtes. Inkluderer situasjoner der samhandling mellom ulike ressurser er nødvendig.</td>
      <td></td>
    </tr>
    <tr>
      <td>leveringssted</td>
      <td>Behandlingssted for levering av pasienter.</td>
      <td></td>
    </tr>
    <tr>
      <td>kontrollpunkt</td>
      <td>Bemannet punkt for ulike typer kontroll, inkludert kontroll av tilgang til avgrensede områder, registrering av personer som evakueres (evakueringspunkt) etc.</td>
      <td></td>
    </tr>
    <tr>
      <td>kommandoplass</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>innsatsledersKO</td>
      <td>Stedet hvor innsatslederne fra brann, politi og helse samles for å lede og koordinere innsatsen under en hendelse. Dette fungerer som et taktisk knutepunkt for informasjonsutveksling og beslutningstaking. (IL-KO).</td>
      <td></td>
    </tr>
    <tr>
      <td>helsehjelp</td>
      <td>Et dedikert område på eller nær et skadested hvor medisinsk behandling gis til skadde eller syke personer. Kan inkludere fasiliteter for førstehjelp og mer omfattende medisinsk hjelp.</td>
      <td></td>
    </tr>
    <tr>
      <td>triage</td>
      <td>Arbeidsprosess med hensikt å bestemme prioritering til behandling og transport basert på hvor alvorlig pasientenes medisinske tilstand er (Helsedirektoratet)</td>
      <td></td>
    </tr>
    <tr>
      <td>dekontaminering</td>
      <td>Dekontaminasjon: fjerning av forurensninger (kontaminasjoner) som har spredt seg innen et begrenset område. Slike forurensninger kan finnes på faste overflater av ulik type, i væsker eller i gasser. De kan bestå av giftige eller miljøresistente kjemikalier, mikroorganismer (bakterier o.l.) og av radioaktive substanser (SNL).</td>
      <td></td>
    </tr>
    <tr>
      <td>samleplass</td>
      <td>Inkluderer sampleplass for døde, skadde, uskadde, vitner, berørte etc.</td>
      <td></td>
    </tr>
    <tr>
      <td>mottakssenter</td>
      <td>Sted hvor man mottar et større antall evakuerte og/ eller skadde fra en hendelse på sjøen eller i utlandet. Mottakssenteret kan også benyttes som en samleplass for evakuerte eller skadde eller som et evakueringspunkt dersom det er hensiktsmessig (PBS 1).</td>
      <td></td>
    </tr>
    <tr>
      <td>evakuerteOgPårørendesenter</td>
      <td>Oppholdssted for evakuerte som ikke er skadet, samt oppmøtested for pårørende.</td>
      <td></td>
    </tr>
    <tr>
      <td>presseOgMedia</td>
      <td>Et dedikert område for håndtering av mediekontakt under hendelser eller operasjoner, hvor journalister kan få informasjon.</td>
      <td></td>
    </tr>
    <tr>
      <td>observasjonspost</td>
      <td>En strategisk plassert posisjon for overvåking og innsamling av informasjon om et bestemt område, ofte brukt til å identifisere risiko, observere hendelser eller koordinere respons.</td>
      <td></td>
    </tr>
    <tr>
      <td>helikopterlandingsplass</td>
      <td>Et tilrettelagt område for trygg landing og avgang av helikoptre, ofte brukt i redningsarbeid, beredskap eller transport til vanskelig tilgjengelige steder.</td>
      <td></td>
    </tr>
    <tr>
      <td>sambandsinstallasjon</td>
      <td>En teknisk installasjon som muliggjør kommunikasjon og informasjonsdeling, ofte brukt i nødetatens og beredskapsaktørers arbeid for å sikre effektiv koordinering.</td>
      <td></td>
    </tr>
    <tr>
      <td>depot</td>
      <td>Lager (opprettet for håndtering av hendelsen) der det oppbevares større mengder materiell for senere bruk.</td>
      <td></td>
    </tr>
    <tr>
      <td>parkeringsplass</td>
      <td>Parkeringsplass</td>
      <td></td>
    </tr>
    <tr>
      <td>kjørerute</td>
      <td>Angivelse av definert kjørerute fra ressursens lokasjon til hendelsessted. Innhentet fra relevant tjeneste.</td>
      <td></td>
    </tr>
    <tr>
      <td>sikkerRute</td>
      <td>Sikker rute for nødetatene inn og ut fra hendelsessted (inkl. for helsepersonell som skal inn til skadde personer, samt evakueringslinje/akse, jf. Håndbok for redningstjeneste). Inkluderer sikker innpå marsj (polititerminologi.).</td>
      <td></td>
    </tr>
    <tr>
      <td>avsperring</td>
      <td>Sperringstiltak oppsatt ifm. en hendelse som marker definerte områder hvor kun nødetater og annet autorisert personell kan oppholde seg. Avsperring settes i kartet iht. etablerte prosedyrer for nødetatene.</td>
      <td></td>
    </tr>
    <tr>
      <td>evakueringssone</td>
      <td>Sone som personer skal evakueres fra.</td>
      <td></td>
    </tr>
    <tr>
      <td>søketeigsone</td>
      <td>Definert område hvor det søkes etter savnede. Merkes iht gjeldende regler for søkeoppdrag (Se Nasjonal veileder søk etter savnet person på land (2022)).</td>
      <td></td>
    </tr>
    <tr>
      <td>faresone</td>
      <td>Definerte områder rundt hendelsen som indikerer grad av risiko for de som oppholder seg der.</td>
      <td></td>
    </tr>
    <tr>
      <td>sikring</td>
      <td>Forebyggende tiltak i forbindelse med brann, flom, utslipp etc.</td>
      <td></td>
    </tr>
    <tr>
      <td>arbeidsområde</td>
      <td>Område som avgrenses for nødetatenes særskilte tiltak under håndteringen av hendelsen.</td>
      <td></td>
    </tr>
    <tr>
      <td>slukking</td>
      <td>Prosessen med å bekjempe og eliminere brann ved hjelp av ulike metoder og utstyr for å stoppe brannens spredning og redusere skadeomfanget.</td>
      <td></td>
    </tr>
    <tr>
      <td>vannbombing</td>
      <td>En metode for brannslukking hvor store mengder vann slippes fra fly eller helikoptre over brannområder, spesielt effektivt ved skogbranner.</td>
      <td></td>
    </tr>
    <tr>
      <td>begrensningslinjeVåt</td>
      <td>En fysisk eller strategisk linje etablert for å hindre videre spredning av brann, ofte ved bruk av naturlige barrierer eller opprettede brannlinjer (Bruk av vann).</td>
      <td></td>
    </tr>
    <tr>
      <td>begrensningslinjeTørr</td>
      <td>En fysisk eller strategisk linje etablert for å hindre videre spredning av brann, ofte ved bruk av naturlige barrierer eller opprettede brannlinjer (uten bruk av vann).</td>
      <td></td>
    </tr>
    <tr>
      <td>vannslange</td>
      <td>Slange brukt i brannslukking for å transportere og levere vann til brannstedet.</td>
      <td></td>
    </tr>
    <tr>
      <td>vannpumpe</td>
      <td>Pumpe brukt i brannslukking for å transportere og levere vann til brannstedet.</td>
      <td></td>
    </tr>
    <tr>
      <td>sektorgrense</td>
      <td>En definert avgrensning mellom ulike sektorer på et skadested, som brukes for å organisere og koordinere innsatsen effektivt.</td>
      <td></td>
    </tr>
    <tr>
      <td>referansesystem</td>
      <td>System som brukes for å identifisere og beskrive spesifikke steder innenfor et område. Brukes ofte for koordinering, spesielt i nødsituasjoner eller komplekse omgivelser.</td>
      <td></td>
    </tr>
    <tr>
      <td>annetTiltak</td>
      <td>Ikke forhåndsdefinerte tiltak</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Status

**Definisjon:** En beskrivelse av tilstanden for fremdrift i tiltaket.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>planlagt</td>
      <td>Tiltaket er planlagt.</td>
      <td></td>
    </tr>
    <tr>
      <td>pågåendeEllerAktivt</td>
      <td>Tiltaket er pågående eller aktivt.</td>
      <td></td>
    </tr>
    <tr>
      <td>gjennomførtEllerAvsluttet</td>
      <td>Tiltaket er gjennomført eller avsluttet.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeFaresone

**Definisjon:** Kategorier av faresone angitt med farge.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>rødSone</td>
      <td>Område med høy risiko for liv/helse.</td>
      <td></td>
    </tr>
    <tr>
      <td>gulSone</td>
      <td>Område med risiko for liv/helse.</td>
      <td></td>
    </tr>
    <tr>
      <td>grønnSone</td>
      <td>Område med lav risiko for liv/helse.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeRute

**Definisjon:** En beskrivelse om det er enveis eller toveis kjøreretning.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>enveis</td>
      <td>Man kan bare kjøre i en retning.</td>
      <td></td>
    </tr>
    <tr>
      <td>toveis</td>
      <td>Man kan bare kjøre i begge retninger.</td>
      <td></td>
    </tr>
    <tr>
      <td>ikkeSatt</td>
      <td>Kjøreretning er ikke satt.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeKontekst

**Definisjon:** En kategorisering av ulik type kontekst.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>farekilder</td>
      <td>Identifisert kilde som kan utgjøre en fare for spredning av risiko under håndteringen av en hendelse, f. eks. eksplosiver, radioaktiv agens etc.</td>
      <td></td>
    </tr>
    <tr>
      <td>beskyttelsesverdigInfrastruktur</td>
      <td>Identifisert infrastruktur som kan utsettes for økt risiko som følge av hendelsen.</td>
      <td></td>
    </tr>
    <tr>
      <td>sårbartObjekt</td>
      <td>Objekter som kan være spesielt sårbare som følge av hendelsen, slik som skoler, barnehager, sykehjem, kulturminner etc.</td>
      <td></td>
    </tr>
    <tr>
      <td>ødelagtInfrastruktur</td>
      <td>Ødelagt infrastruktur som aktørene i hendelsen bør vite om.</td>
      <td></td>
    </tr>
    <tr>
      <td>folkeansamling</td>
      <td>Konsentrasjon av mennesker, f.eks. knyttet til uteliv, arrangementer o.l.</td>
      <td></td>
    </tr>
    <tr>
      <td>hinderSperring</td>
      <td>Fysisk hindring/sperring som kan påvirke fremkommeligheten under en hendelse uten å være en del av selve hendelsen, f.eks. veltede trær, veisperringer eller ødelagte broer som hindrer transport og evakuering.</td>
      <td></td>
    </tr>
    <tr>
      <td>spenningsløsKraftledning</td>
      <td>Kraftledning som er frakoblet strømnettet og dermed ikke lenger utgjør fare for elektrisk støt. Brukes som varsel i hendelseshåndtering for å informere om at det er trygt å bevege seg i nærheten eller under ledningen, for eksempel ved en togulykke.</td>
      <td></td>
    </tr>
    <tr>
      <td>annenKontekst</td>
      <td>Kontekstuell informasjon som ikke inngår i forhåndsdefinerte kategorier.</td>
      <td></td>
    </tr>
  </tbody>
</table>
