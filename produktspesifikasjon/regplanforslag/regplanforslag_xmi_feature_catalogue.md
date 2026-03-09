#### FellesegenskaperKart (abstrakt)

abstrakt objekttype som bærer de egenskapene fra SOSI_Objekt i SOSI Del 1 som er anvendt på stedfesta objekttyper (kartobjekter) i datamodellen.<br />I SOSI Del 1 er SOSI_Objekt en abstrakt objekttype som bærer sentrale egenskaper som er anbefalt for bruk i produktspesifikasjoner.

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
      <td>unik identifikasjon av et dataobjekt.<br /><br />Systemegenskap som ikke skal kunne endres av brukerne</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
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
      <td><strong>identifikasjon.lokalId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>lokal identifikator av et objekt<br />Skal være en uuid, slik at den er unik, uavhengig av navnerommet</td>
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
      <td><strong>identifikasjon.navnerom</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navnerom som unikt identifiserer datakilden til et objekt.<br />Navnerom anbefales å være en http-URI og må være registrert i data.geonorge.no<br />For plan anbefales navnerommet <a href="http://data.geonorge.no/sosi/plan">http://data.geonorge.no/sosi/plan</a></td>
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
      <td><strong>identifikasjon.versjonId</strong></td>
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

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>oppdateringsdato</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>tidspunkt for siste endring på dataobjektet.<br /><br />Systemegenskap som ikke skal kunne endres av brukerne</td>
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
      <td><strong>førsteDigitaliseringsdato</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>dato når en representasjon av objektet i digital form første gang ble etablert</td>
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
      <td><strong>kvalitet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>beskrivelse av kvaliteten på stedfestingen</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Posisjonskvalitet</td>
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
      <td><strong>kvalitet.datafangstmetode</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Datafangstmetode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/datafangstmetode">https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/datafangstmetode</a></td>
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
      <td><strong>kvalitet.nøyaktighet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>punktstandardavviket i grunnriss, oppgitt i cm, for punkter, samt tverravvik for linjer</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
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
      <td><strong>opphav</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>referanse til opphavsmaterialet, kildematerialet, organisasjons/publiseringskilde</td>
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

#### FellesegenskaperArealplan (abstrakt)

abstrakt objekttype som bærer de egenskapene fra SOSI_Objekt i SOSI Del 1 som er anvendt på objekttypen Arealplan

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
      <td>unik identifikasjon av et dataobjekt.<br />Systemegenskap som ikke skal kunne endres av brukerne, men som skal følge dataobjektet og identifisere det i hele dets levetid.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
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
      <td><strong>identifikasjon.lokalId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>lokal identifikator av et objekt<br />Skal være en uuid, slik at den er unik, uavhengig av navnerommet</td>
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
      <td><strong>identifikasjon.navnerom</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navnerom som unikt identifiserer datakilden til et objekt.<br />Navnerom anbefales å være en http-URI og må være registrert i data.geonorge.no<br />For plan anbefales navnerommet <a href="http://data.geonorge.no/sosi/plan">http://data.geonorge.no/sosi/plan</a></td>
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
      <td><strong>identifikasjon.versjonId</strong></td>
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

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>oppdateringsdato</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>tidspunkt for siste endring av dataobjektet.<br />Systemegenskap som ikke skal kunne endres av brukerne</td>
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
      <td><strong>prosesshistorie</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>beskrivelse av de prosesser som dataene er gått gjennom som kan ha betydning for kvaliteten og bruken av dataene</td>
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
      <td><strong>informasjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>generell opplysning<br /><br />Merknad: mulighet til å legge inn utfyllende informasjon om objektet</td>
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
      <td><strong>link</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>referanse til et informasjonselement, enten lokalt eller globalt</td>
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

#### Arealplan

toppobjekt for reguleringsplanen (pbl. §§ 12-1, 12-2 og 12-3).<br />Objektet inneholder informasjon om planen som helhet og med referanser til planens planområder (RpOmråde)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>nasjonalArealplanId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>landsdekkende entydig og unik identifikasjon av en arealplan (pbl. §§ 6-4, 9-1, og 12-1, samt kart- og planforskriften § 9 andre og sjette ledd).<br />Denne identifikatoren tildeles planen når planprosessen starter, og den kan ikke endres undervegs av forslagstiller.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>NasjonalArealplanId</td>
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
      <td><strong>nasjonalArealplanId.kommunenummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode som viser til offisiell nummerering av kommuner<br /><br />Merknad: Det presiseres at kommunenummer alltid skal ha 4 siffer, dvs. eventuelt med ledende null. Kommunenummer benyttes for kobling mot en rekke andre registre som også benytter 4 siffer.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Kommunenummer</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/inndelinger/inndelingsbase/kommunenummer">https://register.geonorge.no/sosi-kodelister/inndelinger/inndelingsbase/kommunenummer</a></td>
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
      <td><strong>nasjonalArealplanId.landkode</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>administrativ enhet for statlig vedtatte planer, landkode = NO, anvendes kun av statlig vedtaksmyndighet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Landkode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- NO – Norge</td>
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
      <td><strong>nasjonalArealplanId.planid</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>entydig identifikasjon av en plan innen vedkommende administrative enhet (pbl. §§ 9-1, 12-1, samt kart- og planforskriften § 9 andre og sjette ledd)</td>
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
      <td><strong>plantype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>type reguleringsplan (pbl. §§ 12-2 og 12-3)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpPlantype</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/rpplantype">https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/rpplantype</a></td>
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
      <td><strong>plannavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>planens offisielle navn</td>
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
      <td><strong>planstatus</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>reguleringsplanens rettsvirkning (pbl.  §§ 12-8 til 12-12, jf § 9-3)<br />For reguleringsplanforslag skal planstatus = Planforslag (2)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Planstatus</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Planforslag – forslag til arealplan er lagt frem for vedtaksmyndigheten (kommunen)</td>
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
      <td><strong>omPlanbestemmelser</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>om planen har bestemmelser (pbl § 12-7), og hvordan disse i så fall er representert<br /><br />Merknad: Egenskapen er gitt nytt navn for at den ikke skal forveksles med forhold knyttet til digitale planbestemmelser.<br />For nye planer er bestemmelsene både på kart og som egen tekst (kode 4)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>OmPlanbestemmelser</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Planbestemmelser både kart og tekst – Planbestemmelser både på kart og som egen tekst.  Dette gleder alltid for nye planer.</td>
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
      <td><strong>lovreferanse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>referanse til lov som planen og bestemmelsene er hjemlet i.<br />For reguleringsplanforslag skal lovreferanse = pbl 2008 (6)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Lovreferanse</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/lovreferanse">https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/lovreferanse</a></td>
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
      <td><strong>lovreferanseBeskrivelse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>tekstlig beskrivelse av hvilken lov planer er vedtatt etter.<br /><br />Merknad: Kan være utfyllende til egenskapen lovereferanse</td>
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
      <td><strong>versjonsdato</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>datoen for denne versjonen av planforslaget (ref. versjonsnummer)</td>
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
      <td><strong>versjonsnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>viser det innsendte planforslagets versjon<br />Kommunen stiller kriterier for når et planforslag skal gis ny versjon</td>
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
      <td><strong>alternativReferanse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>gir anledning til å identifisere ulike planalternativ i en leveranse av planforslaget</td>
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
      <td><strong>forslagsstillerType</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>om forslagsstiller er privat eller offentlig<br />Benyttes for å kunne skille arealplaner i prosess som skal fremmes etter prosessreglene for private planer (pbl. § 12.11) og planer som skal fremmes etter prosessreglene for offentlige planer</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>ForslagsstillerType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- offentlig – offentlig forslagsstiller.  Planen skal fremmes etter prosessreglene for offentlige planer (pbl. § 12-10)<br />- privat – privat forslagsstiller.
Planen skal fremmes etter prosessreglene for private planer (pbl. § 12-11)</td>
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
      <td><strong>planhøring</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>egenskapssett for å holde rede på versoner og alternative planforslag som legges ut til høring og offentlig ettersyn (pbl § 12-9)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Planhøring</td>
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
      <td><strong>planhøring.høringsversjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>planforslaget kan legges ut til høring og offentlig ettersyn flere ganger. Hver publisering gis en versjonsangivelse (f.eks. en dato og/eller et serienummer)</td>
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
      <td><strong>planhøring.høringsalternativ</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>planforslaget kan legges ut til høring og offentlig ettersyn med to eller flere planalternativer</td>
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
      <td><strong>planhøring.høringsstart</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>dato for når høring og offentlig ettersyn starter</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
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
      <td><strong>planhøring.høringsslutt</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>dato for når høring og offentlig ettersyn slutter</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperArealplan

**Assosiasjoner**
RpOmråde – rolle: rpOmråde – kardinalitet: 1..*

#### RpGrense

avgrensingslinje for planomåde (RpOmråde) i reguleringsplan (pbl. §§ 12-1, 12-2 og 12-3)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>avgrensingslinje</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpObjekt

#### RpOmråde

planområde for reguleringsplan (områderegulering eller detaljregulering) (pbl. §§ 12-1, 12-2 og 12-3)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>heleid flategeometri</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_MultiSurface</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpObjekt

**Assosiasjoner**
RpGrense – rolle: avgrensesAv – kardinalitet: 0..*
RpRegulertHøyde – rolle: regulertHøyde – kardinalitet: 0..*
RpBestemmelseMidlByggAnlegg – rolle: midlByggAnlegg – kardinalitet: 0..*
RpDetaljeringSone – rolle: detaljering – kardinalitet: 0..*
RpJuridiskPunkt – rolle: juridiskPunkt – kardinalitet: 0..*
RpArealformålOmråde – rolle: formål – kardinalitet: 1..*
RpInfrastrukturSone – rolle: infrastruktur – kardinalitet: 0..*
RpGjennomføringSone – rolle: gjennomføring – kardinalitet: 0..*
RpFareSone – rolle: fare – kardinalitet: 0..*
RpBestemmelseOmråde – rolle: bestemmelseOmråde – kardinalitet: 0..*
RpBåndleggingSone – rolle: båndlegging – kardinalitet: 0..*
RpSikringSone – rolle: sikring – kardinalitet: 0..*
RpStøySone – rolle: støy – kardinalitet: 0..*
RpHensynSone – kardinalitet: 0
RpAngittHensynSone – rolle: angittHensyn – kardinalitet: 0..*
RpJuridiskLinje – rolle: juridiskLinje – kardinalitet: 0..*

#### RpObjekt (abstrakt)

abstrakt objekttype som omfatter alle typer kartobjekter i en reguleringsplan.<br />Objekttypen er utstyrt med egenskaper som identifiserer hviken arealplan og hvilket kartlag det enkelte kartobjekt tilhører

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>nasjonalArealplanId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>landsdekkende entydig og unik identifikasjon for en arealplan.<br />I forvaltningsløsnignene kan den brukes som koblingsnøkkel mellom kartobjekene og den arealplanen de tilhører.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>NasjonalArealplanId</td>
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
      <td><strong>nasjonalArealplanId.kommunenummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode som viser til offisiell nummerering av kommuner<br /><br />Merknad: Det presiseres at kommunenummer alltid skal ha 4 siffer, dvs. eventuelt med ledende null. Kommunenummer benyttes for kobling mot en rekke andre registre som også benytter 4 siffer.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Kommunenummer</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/inndelinger/inndelingsbase/kommunenummer">https://register.geonorge.no/sosi-kodelister/inndelinger/inndelingsbase/kommunenummer</a></td>
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
      <td><strong>nasjonalArealplanId.landkode</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>administrativ enhet for statlig vedtatte planer, landkode = NO, anvendes kun av statlig vedtaksmyndighet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Landkode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- NO – Norge</td>
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
      <td><strong>nasjonalArealplanId.planid</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>entydig identifikasjon av en plan innen vedkommende administrative enhet (pbl. §§ 9-1, 12-1, samt kart- og planforskriften § 9 andre og sjette ledd)</td>
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
      <td><strong>vertikalnivå</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>beliggenheten i forhold til jordoverflaten (pbl. § 19-1 sjette ledd, § 20-1 andre og femte ledd og § 22 og § 28-2) for planområdet med tilhørende kartobjekt</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Vertikalnivå</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Under grunnen (tunnel) – Under bakken, f.eks. tunnel.<br />- På grunnen/vannoverflate – På bakken eller på vannoverflata<br />- Over grunnen (bru) – Over bakken, f.eks. bru.<br />- På bunnen (vann/sjø) – På bunnen av sjø eller innsjø<br />- I vannsøylen</td>
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
      <td><strong>vertikallag</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>identifikasjon av et lag i et vertikalnivå.<br /><br />Når en plan har flere lag i samme vertikalnivå, brukes denne egenskapen for å identifisere hvilket lag kartobjektet tilhører</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Vertikallag</td>
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
      <td><strong>vertikallag.lag</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>identifiserer vertikallag innen samme vertikalnivå</td>
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
      <td><strong>vertikallag.referansehøyde</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>nærmere spesifiering av høydenivået for vertikallaget</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Real</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperKart

#### RpFormålGrense

avgrensingsobjekt for formålsområde (RpArealformålOmråde)<br />Avgrensingslinja skal inneholde informasjon om kvalitet, slik at saksbehandler kan be om tiltak der kvaliteten ikke er tilfredsstillende.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>avgrensingslinje</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpObjekt

#### RpHandlingOmråde

område som konstruksjonen/tiltaket må holde seg innenfor (kart- og planforskriften vedlegg I bokstav c nr. 4 – formål og bestemmelser fastsatt med linjer i reguleringsplan).<br /><br />Merknad: RpHandlingOmråde har samme betydning som byggegrense og anvendes ved fremstilling av planen i 2D.<br />Dersom det også er angitt et 3D-rom som avgrenser tiltaket vertikalt, er dette gitt ved et tilhørende RpHandlingRom. Det må da være samsvar mellom de to geometriene ved at flategeometrien er fotavtrykket (grunnrissprojeksjonen) av romgeometrien.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>områdets flategeometri</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Surface</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpObjekt

**Assosiasjoner**
RpHandlingRom – rolle: rom – kardinalitet: 0..1

#### RpArealformålOmråde

område med angitt arealformål i reguleringsplan (pbl. § 12-5)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>heleid flategeometri</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_MultiSurface</td>
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
      <td><strong>arealformål</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>angivelse av arealformål i reguleringsplan (pbl. § 12-5)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpArealformål</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/rparealformål">https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/rparealformål</a></td>
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
      <td><strong>feltnavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>unik forkortelse for navn på formålsflater i områderegulering og detaljregulering (pbl. § 12-5 første ledd, pbl. § 12-7 nr. 4, samt TEK17 § 5-6 og kap. 8).<br />Feltnavn skal være i samsvar med arealformål og eierform, der arealformålet angis i henhold til kodeliste fra KDD.<br />Feltnavn skal skrives ut på plankartet.<br />Feltnavn brukes som koblingsnøkkel mellom plankartet og planbestemmelsene.</td>
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
      <td><strong>beskrivelse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>beskrivelse kan benyttes der loven gir anledning til detaljering, for eks, "andre anlegg", men der lov/forskrift ikke definerer detaljeringen i form av spesifikke arealformål.</td>
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
      <td><strong>eierform</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>planbestemmelse om eierform (pbl. § 12-7 nr. 14).<br />Eierform angir hvilke arealer det offentlige må sikre seg eiendoms- eller bruksrett til for å få gjennomført planen. Tilsvarende der eierne av bestemte angitte eiendommer er forutsatt å disponere et areal i fellesskap.<br />Eierform skal alltid angis på plankartet når det fra planmyndighetens side er forutsatt at det offentlige skal være eier av grunnen eller ha eksklusiv rett til å disponere arealet, bygningen, konstruksjonen eller anlegget på eiendommen, eller det er det offentlige som skal råde over virksomhet som skal utøves på eiendommen/arealet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>EierformType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- offentlig formål – det offentlige skal være eier av grunnen eller ha eksklusiv rett til å disponere arealet, bygningen, konstruksjonen eller anlegget på eiendommen, eller det offentlige skal råde over virksomhetenom skal utøves på eiendommen/arealet<br />- felles – eierne av bestemt angitte eiendommer skal disponere arealet i felleskap<br />- annen eierform – angir at det ikke er bestemt offentlig eller felles eierform.  Brukes altså som default verdi for arealer som ikke skal ha kodeverdi 1 eller 2. Koden er hverken hjemlet i pbl. § 11-10 nr. 3 eller § 12-7 nr. 14.</td>
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
      <td><strong>utnytting</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>fastsatt grad av utnytting (pbl. § 12-7 nr. 5, samt TEK kap. 5).<br />Benyttes for å regulere bygningers volum og totale areal, sett i forhold til behovet for uteoppholdsareal, belastning på infrastruktur og forholdet til omgivelsene.<br />Dersom utnytting er angitt med flere forekomster skal det referers til ulik utnyttingstype i hver av forekomstene.<br />I områder for kjøpesentre og forretninger skal bruksareal (BRA) alltid brukes til å fastsette grad av utnytting  (TEK § 5-1, 2. ledd). BRA gir oversikt over det samlede arealet for alle plan i en bygning. BRA er derfor hensiktsmessig å bruke i områder for kjøpesentre og forretninger hvor man ønsker å styre størrelsen på bebyggelsen av hensyn til belastningen på omgivelsene.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Utnytting</td>
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
      <td><strong>utnytting.utnyttingstype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>type grad av utnytting (pbl. § 12-7 første ledd nr 5 og TEK17 kap. 5)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Utnyttingstype</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Ikke tillatt å bebygge<br />- Ikke tillatt med ytterligere bebyggelse<br />- BYA – Bebygd areal i kvm etter TEK<br />- %-BYA – Bebygd areal i prosent etter TEK<br />- BRA – Bruksareal i kvm etter TEK<br />- %-BRA – Bruksareal i prosent etter TEK</td>
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
      <td><strong>utnytting.utnyttingstall</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>tallverdi for grad av utnytting (pbl. §12-7 første ledd nr 5 og TEK17 kap. 5)<br />Betydningen av tallet følger av utnyttingstypen</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
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
      <td><strong>utnytting.utnyttingstall_minimum</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>tallverdi for minste utnyttingsgrad (pbl. §12-7 første ledd nr 5 og TEK17 kap 5 )</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
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
      <td><strong>uteoppholdsareal</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>fastsatt minste uteoppholdsareal (MUA).<br />Benyttes for å sikre tilstrekkelige og brukbare arealer til uteopphold med god kvalitet (pbl. § 28-7 tredje ledd og forskrift TEK17 § 5-6)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
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
      <td><strong>avkjørselsbestemmelse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>planbestemmelse om avkjørsel (pbl. § 12-7 nr. 7 og TEK § 8-8)<br /><br />Merknad:  Angir om avkjørsel til formålsområde tillates eller ikke tillates, eller om det i plan og/eller bestemmelser er tillatt avkjørsel via annet formål enn vei (via gangvei, turvei e.l.).  I sistnevnte situasjon knyttes egenskapen til det formålsområdet det er tillatt å passere</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Avkjørselsbestemmelse</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Avkjørsel tillatt – Avkjørsel er tillatt<br />- Avkjørsel ikke tillatt – Avkjørsel er ikke tillatt</td>
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
      <td><strong>byggverkbestemmelse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>henvisning til planbestemmelse om bygningers plassering, utforming mv. (pbl. § 12-7 nr. 1 og 2, samt TEK kap. 7 og § 8-3)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Byggverkbestemmelse</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Fastsatt plassering – Fastsatt plassering av bygning<br />- Fastsatt høyde – Fastsatt høyde av bygning<br />- Fastsatt plassering/høyde – Fastsatt plassering/høyde av bygning<br />- Fastsatt møneretning – Fastsatt møneretning av bygning<br />- Fastsatt plassering/møneretning – Fastsatt plassering/møneretning av bygning<br />- Fastsatt plassering/høyde/møneretning – Fastsatt plassering/høyde/møneretning av bygning<br />- Fastsatt utforming – Fastsatt utforming av bygning</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpObjekt

**Assosiasjoner**
RpFormålGrense – rolle: avgrensesAv – kardinalitet: 0..*
RpHandlingOmråde – rolle: handlingsområde – kardinalitet: 0..*

#### RpHandlingRom

handlingsrom i 3D for RpHandlingOmråde.<br />Konstruksjonen/tiltaket må holde seg innenfor handlingrommet, i henhold til de tilhørende planbestemmelsene

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>rom</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>lukket romgeometri i 3D</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Solid</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpObjekt

#### RpBåndleggingSone

hensynssone for båndlegging i reguleringsplan (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav d)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>båndlegging</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode for type båndlegging i hensynssone for båndlegging (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav d)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpBåndleggingSoneType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Båndlegging for regulering etter pbl. – Båndlegging for regulering etter plan- og bygningsloven<br />- Båndlegging etter naturvernloven – Båndlegging etter lov om naturvern<br />- Båndlegging etter kulturminneloven – Båndlegging etter lov om kulturminner<br />- Båndlegging etter markaloven – Båndlegging etter lov om naturområder i Oslo og nærliggende kommuner (markaloven)<br />- Båndlegging etter andre lover<br />- Båndlegging etter vegloven – Båndlegging i henhold til avkjøringsklasser etter vegloven</td>
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
      <td><strong>båndlagtFremTil</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>planbestemmelsen om midlertidig båndlagt i påvente av vedtak etter pbl., eller særlov, med angivelse av hvilke rådighetsbegrensinger som gjelder inntil det er utarbeidet et nytt forvaltningsgrunnlag for arealet (pbl. § 11-8 tredje ledd bokstav d)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpHensynSone

#### RpHensynSone (abstrakt)

områder som angir en hensynssone i reguleringsplan (pbl. § 12-6, jf. § 11-8)<br /><br />Merknad: RpHensynSone er en supertype som ikke skal realiseres. Den er en generalisering som er felles for alle typer hensynssoner i modellen.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>områdets flategeometri</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_MultiSurface</td>
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
      <td><strong>hensynSonenavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>unikt navn som gir entydig identifikasjon av hensynssone i reguleringplan (pbl. § 12-6, jf. § 11-8)</td>
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
      <td><strong>beskrivelse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>beskrivelse kan benyttes der loven gir anledning til detaljering, f.eks. "andre anlegg", men der lov/forskrift ikke definerer detaljeringen i form av spesifikke arealformål</td>
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
RpObjekt

**Assosiasjoner**
RpHensynRom – rolle: rom – kardinalitet: 0..1

#### RpInfrastrukturSone

hensynssone for særlige krav til infrastruktur i reguleringsplan (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav b)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>infrastruktur</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode for særlige krav til infrastruktur (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav b)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpInfrastrukturSoneType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Krav vedrørende infrastruktur – Krav vedrørende infrastruktur ( pbl §11-8, bokstav b)<br />- Rekkefølgekrav infrastruktur – Rekkefølgekrav til teknisk infrastruktur (pbl § 11-9, nr 4 )<br />- Rekkefølgekrav samfunnservice – Rekkefølgekrav til samfunnservice (pbl § 11-9, nr 4 )<br />- Rekkefølgekrav grønnstruktur – Rekkefølgekrav til grønnstruktur (pbl § 11-9, nr 4 )</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpHensynSone

#### RpAngittHensynSone

hensynssone for nærmere angitt hensyn i reguleringsplan (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav c)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>angittHensyn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode for type angitt hensyn i hensynssone for nærmere angitt hensyn (pbl. §12-6, jf. § 11-8 tredje ledd bokstav c)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpAngittHensynSoneType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Hensyn landbruk<br />- Hensyn reindrift<br />- Hensyn friluftsliv<br />- Hensyn grønnstruktur<br />- Hensyn landskap<br />- Bevaring naturmiljø<br />- Bevaring kulturmiljø<br />- Randområder til nasjonalpark/landskapsvernområde – Sikring av randområder til nasjonalpark eller landskapsvernområde<br />- Sikring av mineralressurser – sikring av mineralressurser</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpHensynSone

#### RpStøySone

hensynssone for støy i reguleringsplan (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav a)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>støy</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode for type støy i hensynssone for støy (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav a)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpStøySoneType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Rød sone – Rød sone iht. T-1442<br />- Gul sone – Gul sone iht. T-1442<br />- Grønn sone – Grønn sone iht. T-1442<br />- Andre støysoner</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpHensynSone

#### RpFareSone

hensynssone for fare i reguleringsplan (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav a)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>fare</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode for type fare i hensynssone for fare (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav a)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpFareSoneType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Ras- og skredfare<br />- Flomfare<br />- Radon – Radonfare<br />- Brann-/eksplosjonsfare – Brann- og eksplosjonsfare<br />- Skytebane<br />- Høyspenningsanlegg (inkl høyspentkabler) – Høyspenningsanlegg, inkl høyspentkabler<br />- Sone for militær virksomhet<br />- Annen fare</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpHensynSone

#### RpGjennomføringSone

hensynssone med bestemmelse om at flere eiendommer skal undergis felles planlegging med bruk av særskilte gjennomføringsvirkemidler (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav e andre ledd)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>gjennomføring</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode for type særskilte gjennomføringsvirkemidler</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpGjennomføringSoneType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Krav om felles planlegging – krav om felles planlegging for flere eiendommer, herunder med særlige samarbeids- eller eierformer<br />- Omforming – krav om målrettet og særskilt områdevis planlegging og gjennomføring for omforming<br />- Krav om grunneierfinansiering av infrastruktur – Krav om grunneierfinansiering av infrastruktur etter pbl. § 12 A-1<br />- Krav om flytting av infrastruktur – Krav om flytting av infrastruktur for å frigjøre areal til utbyggingsformål etter § 12 A-13</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpHensynSone

#### RpDetaljeringSone

hensynssone for videreføring av reguleringsplan (pbl. § 12-6, jf. §11-8 tredje ledd bokstav f).<br />Kan benyttes i områderegulering for å angi videreføring av detaljregulering. Skal ikke anvendes i detaljregulering.<br /><br />Merknad: Hensynssonen skal ikke kunne fremstilles i 3D.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>detaljering</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode som angir videreføring av gjeldende reguleringsplan (pbl. § 12-6, jf. §11-8 tredje ledd bokstav f)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpDetaljeringSoneType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Reguleringsplan skal fortsatt gjelde – eksisterende reguleringsplan skal fortsatt gjelde</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpHensynSone

#### RpSikringSone

hensynssone for sikring i reguleringsplan (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav a)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>sikring</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode for type sikring i hensynssone for sikring (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav a)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpSikringSoneType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Nedslagsfelt drikkevann – sikring av nedslagsfelt for drikkevann, område, over og under bakken, som vannet i råvannskilden kommer fra. Drikkevannsforskriften bruker begrepet "vanntilsigsområde"<br />- Område for grunnvannsforsyning – sikring av vannforekomst i grunnen, fra sand og grusressurser samt vannførende berggrunn<br />- Byggeforbud rundt veg, bane og flyplass – sikkerhetssone langs veg, bane og flyplass av hensyn til fare og trafikksikkerhet<br />- Andre sikringssoner – sikkerhetssone langs andre formål<br />- Frisikt – frisiktsone ihht vegloven</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpHensynSone

#### RpHensynRom

hensynsrom i 3D for RpHensynSone<br />Hensynsrommet tilhører alltid en hensynssone, som er en av subtypene til den abstrakte supertypen RpHensynSone, dvs. en av disse: RpStøySone, RpSikringSone, RpFareSone, RpBåndleggingSone, RpAngittHensynSone, RpInfrastrukturSone eller RpGjennomføringSone.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>rom</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>lukket romgeometri i 3D</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Solid</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpObjekt

#### RpBestemmelseOmråde

område for stedfesting av bestemmelser som ikke kan knyttes til et formålsområde eller en hensynsone (pbl. § 12-7 nr. 1-14)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>områdets flategeometri</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_MultiSurface</td>
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
      <td><strong>bestemmelseHjemmel</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Henvisning til hjemmel ihht. pbl. § 12-7<br />Det kan unntaksvis angis flere hjemler, der det er nødvendig for å unngå flere geometrisk identiske områder</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpBestemmelseHjemmel</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- utforming – Pbl. § 12-7 nr. 1 om utforming, herunder estetiske krav, og bruk av arealer, bygninger og anlegg i planområdet<br />- vilkår for bruk av arealer, bygninger og anlegg – Pbl. § 12-7 nr. 2 om vilkår for bruk av arealer, bygninger og anlegg i planområdet, eller forbud mot former for bruk, herunder byggegrenser, for å fremme eller sikre formålet med planen, avveie interesser og ivareta ulike hensyn i eller av hensyn til forhold utenfor planområdet<br />- grenseverdier/krav til forurensning og miljøkvalitet – Pbl. § 12-7 nr. 3 om grenseverdier for tillatt forurensning og andre krav til miljøkvalitet i planområdet, samt tiltak og krav til ny og pågående virksomhet i eller av hensyn til forhold utenfor planområdet for å forebygge eller begrense forurensning<br />- funksjons- og kvalitetskrav til bygninger, anlegg og utearealer – Pbl. § 12-7 nr. 4 om funksjons- og kvalitetskrav til bygninger, anlegg og utearealer, herunder krav for å sikre hensynet til helse, miljø, sikkerhet, universell utforming og barns særlige behov for leke- og uteoppholdsareal<br />- antall boliger, boligstørrelse, tilgjengelighet, mm – Pbl. § 12-7 nr. 5 om antallet boliger i et område, største og minste boligstørrelse, og nærmere krav til tilgjengelighet og boligens utforming der det er hensiktsmessig for spesielle behov<br />- sikre verneverdier i bygninger, andre kulturminner og kulturmiljøer – Pbl § 12-7 nr. 6 om bestemmelser for å sikre verneverdier i bygninger, andre kulturminner, og kulturmiljøer, herunder vern av fasade, materialbruk og interiør, samt sikre naturtyper og annen verdifull natur<br />- trafikkregulerende tiltak og parkeringsbestemmelser – Pbl. § 12-7 nr. 7 om trafikkregulerende tiltak og parkeringsbestemmelser for bil og sykkelparkering, herunder øvre og nedre grense for parkeringsdekning<br />- krav om tilrettelegging for vannbåren varme – Pbl. § 12-7 nr. 8 om krav om tilrettelegging for forsyning av vannbåren varme til ny bebyggelse, og at det er tilknytningsplikt etter § 27-5<br />- retningslinjer for særlige drifts- og skjøtselstiltak – Pbl. § 12-7 nr. 9 om retningslinjer for særlige drifts- og skjøtselstiltak innenfor arealformålene nr. 3, 5 og 6 i § 12-5<br />- krav om særskilt rekkefølge for gjennomføring av tiltak – Pbl. § 12-7 nr. 10 om krav om særskilt rekkefølge for gjennomføring av tiltak etter planen, og at utbygging av et område ikke kan finne sted før tekniske anlegg og samfunnstjenester som energiforsyning, transport og vegnett, helse- og sosialtjenester, helse- og omsorgstjenester, barnehager, friområder, skoler mv. er tilstrekkelig etablert<br />- krav om detaljregulering – Pbl. § 12-7 nr. 11 om krav om detaljregulering for deler av planområdet eller bestemte typer av tiltak, og retningslinjer for slik plan<br />- krav om nærmere undersøkelser, overvåking og klargjøring av virkninger – Pbl. § 12-7 nr. 12 om krav om nærmere undersøkelser før gjennomføring av planen, samt undersøkelser med sikte på å overvåke og klargjøre virkninger for miljø, helse, sikkerhet, tilgjengelighet for alle, og andre samfunnsinteresser, ved gjennomføring av planen og enkelttiltak i denne<br />- krav om fordeling av planskapt netto verdiøkning – Pbl. § 12-7 nr. 13 om krav om fordeling av planskapt netto verdiøkning ved ulike felles tiltak innenfor en nærmere bestemt del av planområdet i henhold til jordskifteloven § 3-30<br />- hvilke arealer som skal være til offentlige formål eller fellesareal – Pbl. § 12-7 nr. 14 om hvilke arealer som skal være til offentlige formål eller fellesareal</td>
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
      <td><strong>bestemmelseOmrådeNavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>unikt navn på bestemmelseOmråde<br />Navnet skal være på formen #</td>
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
RpObjekt

**Assosiasjoner**
RpBestemmelseRom – rolle: rom – kardinalitet: 0..1
RpBestemmelseRegTerreng – rolle: regulertTerreng – kardinalitet: 0..*

#### RpBestemmelseRom

bestemmelserom i 3D for RpBestemmelseOmråde

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>rom</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>lukket romgeometri i 3D</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Solid</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpObjekt

#### RpBestemmelseMidlByggAnlegg

bestemmelsesområde for midlertidig bygge- og anlegg, jfr. pbl $ 12-7 nr. 1.<br /><br />Merknad:<br />Dette er et bestemmelsesområde, men av hensyn til å kunne forvalte området uavhengig av resten av planen, håndteres det som en egen objekttype.<br />Hjemmel for bruk av areal til ulike formål over tid er pbl. § 12-7 nr. 1 om bruk av arealer. I planens bestemmelser skal det klart angis hvilken hendelse eller hvilket tidspunkt det midlertidige bygge- og anleggsområdet opphører. Når det midlertidige bygge- og anleggsområdet er opphørt, skal det ikke lenger inngå i planen.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>områdets flategeometri</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_MultiSurface</td>
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
      <td><strong>bestemmelseOmrådeNavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>unikt navn på midlertidig bygg- og anleggsområde</td>
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
      <td><strong>gyldigTilDato</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>utløpsdato for bestemmelseområdet. Etter denne skal det midlertidige bestemmelseområdet fjernes.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
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
      <td><strong>avgjørelsesdato</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>dato for vedtak/avgjørelse av enkeltvedtak</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
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
      <td><strong>saksnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>entydig nummer for enkeltsaker og enkeltvedtak</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Saksnummer</td>
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
      <td><strong>saksnummer.saksår</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Årstallet saken ble initiert</td>
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
      <td><strong>saksnummer.sakssekvensnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>løpenummer for saken innenfor året.<br /><br />NB! attributtnavnet forandret fra sekvensnummer til sakssekvensnummer desember 2011, for å tilpasses NOARK 5.</td>
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

Relasjoner

**Arv**
RpObjekt

**Assosiasjoner**
RpBestemmelseRom – rolle: rom – kardinalitet: 0..1
RpBestemmelseRegTerreng – rolle: regulertTerreng – kardinalitet: 0..*

#### RpBestemmelseRegTerreng

regulert terrengoverflate slik det fremgår av planen.<br /><br />Merknad: Det regulerte terrenget er å betrakte som en bestemmelse som må knyttes til et RpBestemmelseOmråde

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>overflate</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>angivelse av terrenget slik det skal være når tiltaket er gjennomført eller slik det maksimalt/minimalt kan utnyttes.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Surface</td>
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
      <td><strong>overflateType</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>hvilke føringer den gitte overflaten setter for tillatt endring av terrenget</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RegulertOverflateType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- planlagt – overflate som angir terrenget slik det skal ferdigstilles<br />- høyeste – overflate som angir maksimum høyde, dvs maksimal tillatt oppfylling på terrenget<br />- laveste – overflate som angir minimum høyde, dvs maksimal tillatt utgravning av terrenget</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpObjekt

#### RpRegulertHøyde

linje med bestemmelse om regulert høyde (bestemmelse om utforming illustrert på kart, pbl. § 12-7 nr. 1)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>linjeforløp</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kurvegeometri som bestemmer linjas forløp på kartet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
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
      <td><strong>høydeFraPlanbestemmelse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>regulert høyde gitt i planbestemmelser (bestemmelse om utforming illustrert på kart, pbl. § 12-7 nr. 1)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>HøydeFraPlanbestemmelse</td>
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
      <td><strong>høydeFraPlanbestemmelse.regulertHøyde</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>tall for kotehøyde eller høyde over terreng ved bestemmelse om regulert høyde (bestemmelse om utforming illustrert på kart, pbl. § 12-7 nr. 1. )</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Real</td>
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
      <td><strong>høydeFraPlanbestemmelse.typeHøyde</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode som angir hva planbestemmelsen regulerer høyden av</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeHøyde</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- gesimshøyde – høyde til skjæringen mellom ytterveggens ytre flate og takflaten. Der taket er forsynt med et takoppbygg eller parapet som stikker mer enn 0,3 m opp over takflaten, regnes høyden til toppen av takoppbygget/parapetet. Måles i forhold til ferdig planert terrengs gjennomsnittsnivå rundt bygningen (TEK § 6-2)<br />- mønehøyde – høyde til skjæringen mellom to skrå takflater. Måles i forhold til ferdig planert terrengs gjennomsnittsnivå rundt bygningen  (TEK § 6-2)<br />- terrenghøyde – terrengets høyde<br />- planeringshøyde – høyden av ferdig planert terreng</td>
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
      <td><strong>høydeFraPlanbestemmelse.høydereferansesystem</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>referansesystem som høydeverdiene refererer til. Gjeldende høydereferansesystem i Norge er NN2000</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Høydereferansesystem</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- NN2000 – Norsk Null av 2000.
Nytt felles nordisk vertikalt datum, basert på Normaal Amsterdals Peil.</td>
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
      <td><strong>høydeFraPlanbestemmelse.terrengreferanse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>type terrengoverflate som er utgangspunkt for å angi høyde over terreng<br /><br />Kan bare brukes for gesimshøyde og mønehøyde</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Terrengreferanse</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- ferdigPlanertTerreng – gjennomsnittlig nivå av ferdig planert terreng<br />- gatenivå – gatas gjennomsnittsnivå<br />- eksistrendeTerreng – gjennomsnittlig nivå av terreng som ikke er mekanisk behandlet</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpObjekt

#### RpJuridiskPunkt

punkt for juridisk bindende tilleggsinformasjon (pbl. §§ 12-2, 12-3, 12-5, og 12-7)

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
      <td>punkt for stedfesting av objektet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Point</td>
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
      <td><strong>juridiskPunkttype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode for type juridisk punkt i reguleringsplan, jf. pbl. kap. 12</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpJuridiskPunktType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Veistengning/fysisk kjøresperre – Regulert vegstenging<br />- Stenging av avkjørsel – Regulert stengt avkjørsel<br />- Avkjørsel - både inn og utkjøring – Regulert avkjørsel - både inn og utkjøring<br />- Avkjørsel - kun innkjøring – Regulert avkjørsel - kun innkjøring<br />- Avkjørsel - kun utkjøring – Regulert avkjørsel - kun utkjøring<br />- Brukar – Regulert brukar<br />- Tunnelåpning – Regulert tunnelåpning<br />- Eksisterende tre som skal bevares – Regulert bevaring av eksisterende tre<br />- Regulert nytt tre<br />- Regulert møneretning</td>
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
      <td><strong>objektnavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navn til juridisk punkt i plankartet. Anvendes som koblingsnøkkel for å koble kartobjektet (punktet) til planbestemmelsene.</td>
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
      <td><strong>retningsvektor</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>retningsvektor i terrenget</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Vector</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpObjekt

#### RpJuridiskLinje

linje for juridisk bindende tilleggsinformasjon (pbl. §§ 12-2, 12-3, 12-5 og 12-7)

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>linjeforløp</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kurvegeometri som bestemmer linjas forløp på kartet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
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
      <td><strong>juridiskLinjetype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kode for type juridisk linje i reguleringsplan, jf. pbl. kap. 12</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>RpJuridiskLinjeType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Regulert tomtegrense – Regulert eiendomsgrense<br />- Eiendomsgrense som skal oppheves – Eiendomsgrense som oppheves ved vedtak av plan<br />- Bygg, kulturminner, mm. som skal bevares – Bygg som skal bevares (kun bevaringsområder)<br />- Byggegrense – grense mellom arealer som kan bebygges og ikke kan bebygges.<br />- Planlagt bebyggelse – Omriss av planlagt bebyggelse<br />- Bebyggelse som inngår i planen – Omriss av eksisterende bebyggelse som inngår i planen<br />- Bebyggelse som forutsettes fjernet – Omriss av bebyggelse som forutsettes fjernet<br />- Regulert senterlinje<br />- Frisiktlinje – grenselinje for område som skal ha frisikt ved kjøring mot vegkryss
Lengden av frisiktlinjen er avhengig av tillatt hastighet og vegkrysstype<br />- Regulert kant kjørebane<br />- Regulert kjørefelt<br />- Regulert parkeringsfelt<br />- Regulert fotgjengerfelt<br />- Regulert støyskjerm<br />- Regulert støttemur<br />- Sikringsgjerde – Regulert sikringsgjerde<br />- Bru<br />- Tunnel<br />- Måle- og avstandslinje – linje som viser fastsatt avstand eller radius<br />- Strandlinje sjø<br />- Strandlinje vassdrag<br />- Midtlinje vassdrag<br />- Markagrense – Grense for område som omfattes av lov om naturområder i Oslo og nærliggende kommuner (markaloven).</td>
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
      <td><strong>objektnavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navn til juridisk linje i plankartet. Anvendes som koblingsnøkkel for å koble kartobjektet (linja) til planbestemmelsene.</td>
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
RpObjekt

#### RpPåskrift

tekst som er påført plankartet for reguleringsplan (områderegulering og detaljregulering) (pbl. §§ 12-2, 12-3, 12-5 og 12-7)<br />En påskrift presenterer eller gir supplerende informasjon om et kartobjekt. Påskriften skal knyttes til dette kartobjektet ved en assosiasjon, og det skal være posisjonert i samsvar med kartobjektet.<br />Påskriftstypen skal være i samsvar med kartobjektet ihht. restriksjoner i modellen.

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
      <td>representasjonspunkt som knytter påskriften geometrisk til et annet kartobjekt</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Point</td>
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
      <td><strong>tekststreng</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>påskriftens tekstlige innhold</td>
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
      <td><strong>påskriftType</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>hva påskriften i plankartet omhandler.<br />Det må være samsvar mellom denne egenskapen og det kartobjektet som påskriften refererer til.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>PåskriftType</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- feltkode – Feltkode, dvs. navn på et kartobjekt (formålOmråde, hensynsSone, bestemmelseOmråde, osv.)<br />- areal – Arealet av delflaten som påskriften refererer til<br />- utnytting – Utnyttingsgrad for formålsområde.<br />- målsetting – Målsatte avstander i kartet.
Referer til avstandslinje med måltall  (juridisk linje 1259)<br />- radius – Radius på sirkelbue.
Brukes på senterlinje for veg og jernbane.<br />- kotehøyde – Høyde over havet.</td>
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
      <td><strong>tekstplassering</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>egenskap for å plassere og rotere tekst på plankartet.  En videreføring av SOSI-formatets geometritype .TEKST<br />Dersom geometrien er gitt som et punkt, skal det angi startpunktet for teksten, som derfra skal gå vannrett utover til høyre<br />Dersom geometrien er gitt som linje skal teksten starte i første koordinat, og derfra følge linjas retning.<br />Dersom egenskapen ikke er gitt, skal teksten plasseres i representasjonspunktet (posisjon).</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Primitive</td>
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
      <td><strong>formatering</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>egenskapsett for å formatere tekst på plankartet.  En videreføring av utvalgte egenskaper fra SOSI-formatets geometritype .TEKST</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Tekstformatering</td>
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
      <td><strong>formatering.skrifttype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navnet på den skrifttypen eller fonten som benyttes på plankartet.</td>
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
      <td><strong>formatering.fontStørrelse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>fontens størrelse angitt i punkter</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
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
      <td><strong>formatering.referansemålestokk</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>målestokken som teksten er redigert for, dvs. plankartets målestokk. Oppgis som målestokkstall.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RpObjekt

**Assosiasjoner**
RpOmråde – kardinalitet: 0..1
RpArealformålOmråde – rolle: formål – kardinalitet: 0..1
RpBåndleggingSone – rolle: båndlegging – kardinalitet: 0..1
RpHensynSone – kardinalitet: 0
RpInfrastrukturSone – rolle: infrastruktur – kardinalitet: 0..1
RpAngittHensynSone – rolle: angittHensyn – kardinalitet: 0..1
RpStøySone – rolle: støy – kardinalitet: 0..1
RpFareSone – rolle: fare – kardinalitet: 0..1
RpGjennomføringSone – rolle: gjennomføring – kardinalitet: 0..1
RpDetaljeringSone – rolle: detaljering – kardinalitet: 0..1
RpSikringSone – rolle: sikring – kardinalitet: 0..1
RpBestemmelseOmråde – rolle: bestemmelseOmråde – kardinalitet: 0..1
RpBestemmelseMidlByggAnlegg – rolle: midlByggAnlegg – kardinalitet: 0..1
RpRegulertHøyde – rolle: regulertHøyde – kardinalitet: 0..1
RpJuridiskPunkt – rolle: juridiskPunkt – kardinalitet: 0..1
RpJuridiskLinje – rolle: juridiskLinje – kardinalitet: 0..1

### Kodelister

#### «CodeList» Datafangstmetode

**Definisjon:** kodeliste som angir metode for datafangst.
Datafangstmetoden beskriver hvordan selve vektordataene er posisjonert fra et datagrunnlag og ikke prosessen med å innhente det bakenforliggende datagrunnlaget.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/datafangstmetode">https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/datafangstmetode</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Kommunenummer

**Definisjon:** ekstern kodeliste for kommunenummer.
Koder med status Gyldig refererer til dagens kommuner, mens koder med status Ugått referer til utgåtte kommunenummer

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/inndelinger/inndelingsbase/kommunenummer">https://register.geonorge.no/sosi-kodelister/inndelinger/inndelingsbase/kommunenummer</a></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Landkode

**Definisjon:** alfanumerisk kode for nasjonalt nivå / Norge.

Avledet fra "ISO 3166 Codes for the representation of names of countries and their subdivisions"

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
      <td>NO</td>
      <td>Norge</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «CodeList» RpPlantype

**Definisjon:** ekstern kodeliste for type reguleringsplan (pbl. §§ 12-2 og 12-3) ihht til gjeldende lov. Angir om planen er en områdeplan eller detaljplan.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/rpplantype">https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/rpplantype</a></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Planstatus

**Definisjon:** koder for planens virkning (pbl. §§ 9-3, 9-4, og §§ 12-8 til 12-12)
For reguleringsplanforslag skal det angis at det er et planforslag

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
      <td>Planforslag</td>
      <td>forslag til arealplan er lagt frem for vedtaksmyndigheten (kommunen)</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» OmPlanbestemmelser

**Definisjon:** om planen har bestemmelser (pbl. § 12-7), og hvordan disse i så fall er representert.

Merknad: Er gitt nytt navn for at den ikke skal forveksles med forhold knyttet til digitale planbestemmelser.

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
      <td>Planbestemmelser både kart og tekst</td>
      <td>Planbestemmelser både på kart og som egen tekst.  Dette gleder alltid for nye planer.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Lovreferanse

**Definisjon:** ekstern kodeliste for gjeldende pbl.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/lovreferanse">https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/lovreferanse</a></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» ForslagsstillerType

**Definisjon:** koder for om forslagsstiller er privat eller offentlig.

Benyttes for å kunne skille arealplaner i prosess som skal fremmes etter prosessreglene for private planer (pbl. § 12.11) og planer som skal fremmes etter prosessreglene for offentlige planer

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
      <td>offentlig</td>
      <td>offentlig forslagsstiller.  Planen skal fremmes etter prosessreglene for offentlige planer (pbl. § 12-10)</td>
      <td></td>
    </tr>
    <tr>
      <td>privat</td>
      <td>privat forslagsstiller.
Planen skal fremmes etter prosessreglene for private planer (pbl. § 12-11)</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Vertikalnivå

**Definisjon:** kodeliste for planområdets beliggenhet i forhold til jordoverflaten (pbl. § 19-1 sjette ledd, § 20-1 andre og femte ledd og § 22 og § 28-2)

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
      <td>Under grunnen (tunnel)</td>
      <td>Under bakken, f.eks. tunnel.</td>
      <td></td>
    </tr>
    <tr>
      <td>På grunnen/vannoverflate</td>
      <td>På bakken eller på vannoverflata</td>
      <td></td>
    </tr>
    <tr>
      <td>Over grunnen (bru)</td>
      <td>Over bakken, f.eks. bru.</td>
      <td></td>
    </tr>
    <tr>
      <td>På bunnen (vann/sjø)</td>
      <td>På bunnen av sjø eller innsjø</td>
      <td></td>
    </tr>
    <tr>
      <td>I vannsøylen</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «CodeList» RpArealformål

**Definisjon:** ekstern kodeliste for arealformål i reguleringsplan (pbl. § 12-5)

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/rparealformål">https://register.geonorge.no/sosi-kodelister/plan/reguleringsplanforslag/rparealformål</a></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» EierformType

**Definisjon:** kodeliste for eierform.

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
      <td>offentlig formål</td>
      <td>det offentlige skal være eier av grunnen eller ha eksklusiv rett til å disponere arealet, bygningen, konstruksjonen eller anlegget på eiendommen, eller det offentlige skal råde over virksomhetenom skal utøves på eiendommen/arealet</td>
      <td></td>
    </tr>
    <tr>
      <td>felles</td>
      <td>eierne av bestemt angitte eiendommer skal disponere arealet i felleskap</td>
      <td></td>
    </tr>
    <tr>
      <td>annen eierform</td>
      <td>angir at det ikke er bestemt offentlig eller felles eierform.  Brukes altså som default verdi for arealer som ikke skal ha kodeverdi 1 eller 2. Koden er hverken hjemlet i pbl. § 11-10 nr. 3 eller § 12-7 nr. 14.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Utnyttingstype

**Definisjon:** kodeliste for type utnyttingsgrad (pbl. §12-7 første ledd nr 5 og TEK17 kap. 5)

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
      <td>Ikke tillatt å bebygge</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Ikke tillatt med ytterligere bebyggelse</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>BYA</td>
      <td>Bebygd areal i kvm etter TEK</td>
      <td></td>
    </tr>
    <tr>
      <td>%-BYA</td>
      <td>Bebygd areal i prosent etter TEK</td>
      <td></td>
    </tr>
    <tr>
      <td>BRA</td>
      <td>Bruksareal i kvm etter TEK</td>
      <td></td>
    </tr>
    <tr>
      <td>%-BRA</td>
      <td>Bruksareal i prosent etter TEK</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Avkjørselsbestemmelse

**Definisjon:** kodeliste for planbestemmelse om avkjørsel (pbl. §§ 25 og 26 første ledd).

Merknad:
Angir om avkjørsel til formålsområde tillates eller ikke tillates, eller om det i plan / bestemmelser er tillatt avkjørsel via annet formål enn vei (via gangvei, turvei e.l.).  I sistnevnte situasjon knyttes egenskapen til det formålsområde det er tillatt.

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
      <td>Avkjørsel tillatt</td>
      <td>Avkjørsel er tillatt</td>
      <td></td>
    </tr>
    <tr>
      <td>Avkjørsel ikke tillatt</td>
      <td>Avkjørsel er ikke tillatt</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Byggverkbestemmelse

**Definisjon:** kodeliste for henvisning til planbestemmelse om bygningers plassering, utforming mv. ( pbl. §§ 11-10 nr. 1 og 12-7 nr. 1 og 2)

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
      <td>Fastsatt plassering</td>
      <td>Fastsatt plassering av bygning</td>
      <td></td>
    </tr>
    <tr>
      <td>Fastsatt høyde</td>
      <td>Fastsatt høyde av bygning</td>
      <td></td>
    </tr>
    <tr>
      <td>Fastsatt plassering/høyde</td>
      <td>Fastsatt plassering/høyde av bygning</td>
      <td></td>
    </tr>
    <tr>
      <td>Fastsatt møneretning</td>
      <td>Fastsatt møneretning av bygning</td>
      <td></td>
    </tr>
    <tr>
      <td>Fastsatt plassering/møneretning</td>
      <td>Fastsatt plassering/møneretning av bygning</td>
      <td></td>
    </tr>
    <tr>
      <td>Fastsatt plassering/høyde/møneretning</td>
      <td>Fastsatt plassering/høyde/møneretning av bygning</td>
      <td></td>
    </tr>
    <tr>
      <td>Fastsatt utforming</td>
      <td>Fastsatt utforming av bygning</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» RpBåndleggingSoneType

**Definisjon:** uttømmende kodeliste for type båndlegging i hensynssone for båndlegging (pbl. § 11-8 tredje ledd bokstav d)

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
      <td>Båndlegging for regulering etter pbl.</td>
      <td>Båndlegging for regulering etter plan- og bygningsloven</td>
      <td></td>
    </tr>
    <tr>
      <td>Båndlegging etter naturvernloven</td>
      <td>Båndlegging etter lov om naturvern</td>
      <td></td>
    </tr>
    <tr>
      <td>Båndlegging etter kulturminneloven</td>
      <td>Båndlegging etter lov om kulturminner</td>
      <td></td>
    </tr>
    <tr>
      <td>Båndlegging etter markaloven</td>
      <td>Båndlegging etter lov om naturområder i Oslo og nærliggende kommuner (markaloven)</td>
      <td></td>
    </tr>
    <tr>
      <td>Båndlegging etter andre lover</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Båndlegging etter vegloven</td>
      <td>Båndlegging i henhold til avkjøringsklasser etter vegloven</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» RpInfrastrukturSoneType

**Definisjon:** uttømmende kodeliste for type infrastrukturkrav i hensynsone for infrastruktur (pbl. § 11-8, tredje ledd bokstav b,  § 11-9, nr 4 og § 12A-13)

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
      <td>Krav vedrørende infrastruktur</td>
      <td>Krav vedrørende infrastruktur ( pbl §11-8, bokstav b)</td>
      <td></td>
    </tr>
    <tr>
      <td>Rekkefølgekrav infrastruktur</td>
      <td>Rekkefølgekrav til teknisk infrastruktur (pbl § 11-9, nr 4 )</td>
      <td></td>
    </tr>
    <tr>
      <td>Rekkefølgekrav samfunnservice</td>
      <td>Rekkefølgekrav til samfunnservice (pbl § 11-9, nr 4 )</td>
      <td></td>
    </tr>
    <tr>
      <td>Rekkefølgekrav grønnstruktur</td>
      <td>Rekkefølgekrav til grønnstruktur (pbl § 11-9, nr 4 )</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» RpAngittHensynSoneType

**Definisjon:** uttømmende kodeliste for type angitt hensyn i hensynssone for nærmere angitt hensyn  (11-8 tredje ledd bokstav c)

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
      <td>Hensyn landbruk</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Hensyn reindrift</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Hensyn friluftsliv</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Hensyn grønnstruktur</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Hensyn landskap</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Bevaring naturmiljø</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Bevaring kulturmiljø</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Randområder til nasjonalpark/landskapsvernområde</td>
      <td>Sikring av randområder til nasjonalpark eller landskapsvernområde</td>
      <td></td>
    </tr>
    <tr>
      <td>Sikring av mineralressurser</td>
      <td>sikring av mineralressurser</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» RpStøySoneType

**Definisjon:** uttømmende kodeliste for type støy i hensynsone for støy (pbl. § 11-8, tredje ledd bokstav a)

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
      <td>Rød sone</td>
      <td>Rød sone iht. T-1442</td>
      <td></td>
    </tr>
    <tr>
      <td>Gul sone</td>
      <td>Gul sone iht. T-1442</td>
      <td></td>
    </tr>
    <tr>
      <td>Grønn sone</td>
      <td>Grønn sone iht. T-1442</td>
      <td></td>
    </tr>
    <tr>
      <td>Andre støysoner</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» RpFareSoneType

**Definisjon:** uttømmende kodeliste for type fare i hensynssone for fare (pbl. § 11-8, tredje ledd bokstav a)

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
      <td>Ras- og skredfare</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Flomfare</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Radon</td>
      <td>Radonfare</td>
      <td></td>
    </tr>
    <tr>
      <td>Brann-/eksplosjonsfare</td>
      <td>Brann- og eksplosjonsfare</td>
      <td></td>
    </tr>
    <tr>
      <td>Skytebane</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Høyspenningsanlegg (inkl høyspentkabler)</td>
      <td>Høyspenningsanlegg, inkl høyspentkabler</td>
      <td></td>
    </tr>
    <tr>
      <td>Sone for militær virksomhet</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Annen fare</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» RpGjennomføringSoneType

**Definisjon:** uttømmende kodeliste for type særskilte gjennomføringsvirkemidler i gjennomføringssone (pbl. § 11-8 tredje ledd bokstav e andre ledd)

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
      <td>Krav om felles planlegging</td>
      <td>krav om felles planlegging for flere eiendommer, herunder med særlige samarbeids- eller eierformer</td>
      <td></td>
    </tr>
    <tr>
      <td>Omforming</td>
      <td>krav om målrettet og særskilt områdevis planlegging og gjennomføring for omforming</td>
      <td></td>
    </tr>
    <tr>
      <td>Krav om grunneierfinansiering av infrastruktur</td>
      <td>Krav om grunneierfinansiering av infrastruktur etter pbl. § 12 A-1</td>
      <td></td>
    </tr>
    <tr>
      <td>Krav om flytting av infrastruktur</td>
      <td>Krav om flytting av infrastruktur for å frigjøre areal til utbyggingsformål etter § 12 A-13</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» RpDetaljeringSoneType

**Definisjon:** uttømmende kodeliste for type detaljering i detaljeringssone - videreføring av gjeldende reguleringsplan (pbl. § 11-8 tredje ledd bokstav f)

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
      <td>Reguleringsplan skal fortsatt gjelde</td>
      <td>eksisterende reguleringsplan skal fortsatt gjelde</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» RpSikringSoneType

**Definisjon:** uttømmende kodeliste for type sikring i hensynsone for sikring i reguleringsplan (pbl. § 12-6, jf. § 11-8 tredje ledd bokstav a)

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
      <td>Nedslagsfelt drikkevann</td>
      <td>sikring av nedslagsfelt for drikkevann, område, over og under bakken, som vannet i råvannskilden kommer fra. Drikkevannsforskriften bruker begrepet "vanntilsigsområde"</td>
      <td></td>
    </tr>
    <tr>
      <td>Område for grunnvannsforsyning</td>
      <td>sikring av vannforekomst i grunnen, fra sand og grusressurser samt vannførende berggrunn</td>
      <td></td>
    </tr>
    <tr>
      <td>Byggeforbud rundt veg, bane og flyplass</td>
      <td>sikkerhetssone langs veg, bane og flyplass av hensyn til fare og trafikksikkerhet</td>
      <td></td>
    </tr>
    <tr>
      <td>Andre sikringssoner</td>
      <td>sikkerhetssone langs andre formål</td>
      <td></td>
    </tr>
    <tr>
      <td>Frisikt</td>
      <td>frisiktsone ihht vegloven</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» RpBestemmelseHjemmel

**Definisjon:** liste over bestemmelser det er anledning til å gi i henhold til pbl. § 12-7

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
      <td>utforming</td>
      <td>Pbl. § 12-7 nr. 1 om utforming, herunder estetiske krav, og bruk av arealer, bygninger og anlegg i planområdet</td>
      <td></td>
    </tr>
    <tr>
      <td>vilkår for bruk av arealer, bygninger og anlegg</td>
      <td>Pbl. § 12-7 nr. 2 om vilkår for bruk av arealer, bygninger og anlegg i planområdet, eller forbud mot former for bruk, herunder byggegrenser, for å fremme eller sikre formålet med planen, avveie interesser og ivareta ulike hensyn i eller av hensyn til forhold utenfor planområdet</td>
      <td></td>
    </tr>
    <tr>
      <td>grenseverdier/krav til forurensning og miljøkvalitet</td>
      <td>Pbl. § 12-7 nr. 3 om grenseverdier for tillatt forurensning og andre krav til miljøkvalitet i planområdet, samt tiltak og krav til ny og pågående virksomhet i eller av hensyn til forhold utenfor planområdet for å forebygge eller begrense forurensning</td>
      <td></td>
    </tr>
    <tr>
      <td>funksjons- og kvalitetskrav til bygninger, anlegg og utearealer</td>
      <td>Pbl. § 12-7 nr. 4 om funksjons- og kvalitetskrav til bygninger, anlegg og utearealer, herunder krav for å sikre hensynet til helse, miljø, sikkerhet, universell utforming og barns særlige behov for leke- og uteoppholdsareal</td>
      <td></td>
    </tr>
    <tr>
      <td>antall boliger, boligstørrelse, tilgjengelighet, mm</td>
      <td>Pbl. § 12-7 nr. 5 om antallet boliger i et område, største og minste boligstørrelse, og nærmere krav til tilgjengelighet og boligens utforming der det er hensiktsmessig for spesielle behov</td>
      <td></td>
    </tr>
    <tr>
      <td>sikre verneverdier i bygninger, andre kulturminner og kulturmiljøer</td>
      <td>Pbl § 12-7 nr. 6 om bestemmelser for å sikre verneverdier i bygninger, andre kulturminner, og kulturmiljøer, herunder vern av fasade, materialbruk og interiør, samt sikre naturtyper og annen verdifull natur</td>
      <td></td>
    </tr>
    <tr>
      <td>trafikkregulerende tiltak og parkeringsbestemmelser</td>
      <td>Pbl. § 12-7 nr. 7 om trafikkregulerende tiltak og parkeringsbestemmelser for bil og sykkelparkering, herunder øvre og nedre grense for parkeringsdekning</td>
      <td></td>
    </tr>
    <tr>
      <td>krav om tilrettelegging for vannbåren varme</td>
      <td>Pbl. § 12-7 nr. 8 om krav om tilrettelegging for forsyning av vannbåren varme til ny bebyggelse, og at det er tilknytningsplikt etter § 27-5</td>
      <td></td>
    </tr>
    <tr>
      <td>retningslinjer for særlige drifts- og skjøtselstiltak</td>
      <td>Pbl. § 12-7 nr. 9 om retningslinjer for særlige drifts- og skjøtselstiltak innenfor arealformålene nr. 3, 5 og 6 i § 12-5</td>
      <td></td>
    </tr>
    <tr>
      <td>krav om særskilt rekkefølge for gjennomføring av tiltak</td>
      <td>Pbl. § 12-7 nr. 10 om krav om særskilt rekkefølge for gjennomføring av tiltak etter planen, og at utbygging av et område ikke kan finne sted før tekniske anlegg og samfunnstjenester som energiforsyning, transport og vegnett, helse- og sosialtjenester, helse- og omsorgstjenester, barnehager, friområder, skoler mv. er tilstrekkelig etablert</td>
      <td></td>
    </tr>
    <tr>
      <td>krav om detaljregulering</td>
      <td>Pbl. § 12-7 nr. 11 om krav om detaljregulering for deler av planområdet eller bestemte typer av tiltak, og retningslinjer for slik plan</td>
      <td></td>
    </tr>
    <tr>
      <td>krav om nærmere undersøkelser, overvåking og klargjøring av virkninger</td>
      <td>Pbl. § 12-7 nr. 12 om krav om nærmere undersøkelser før gjennomføring av planen, samt undersøkelser med sikte på å overvåke og klargjøre virkninger for miljø, helse, sikkerhet, tilgjengelighet for alle, og andre samfunnsinteresser, ved gjennomføring av planen og enkelttiltak i denne</td>
      <td></td>
    </tr>
    <tr>
      <td>krav om fordeling av planskapt netto verdiøkning</td>
      <td>Pbl. § 12-7 nr. 13 om krav om fordeling av planskapt netto verdiøkning ved ulike felles tiltak innenfor en nærmere bestemt del av planområdet i henhold til jordskifteloven § 3-30</td>
      <td></td>
    </tr>
    <tr>
      <td>hvilke arealer som skal være til offentlige formål eller fellesareal</td>
      <td>Pbl. § 12-7 nr. 14 om hvilke arealer som skal være til offentlige formål eller fellesareal</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» RegulertOverflateType

**Definisjon:** hvilke føringer den gitte overflaten setter for tillatt endring av terrenget

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
      <td>overflate som angir terrenget slik det skal ferdigstilles</td>
      <td></td>
    </tr>
    <tr>
      <td>høyeste</td>
      <td>overflate som angir maksimum høyde, dvs maksimal tillatt oppfylling på terrenget</td>
      <td></td>
    </tr>
    <tr>
      <td>laveste</td>
      <td>overflate som angir minimum høyde, dvs maksimal tillatt utgravning av terrenget</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» TypeHøyde

**Definisjon:** kodeliste for å spesifisere hva slags høyde som er regulert

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
      <td>gesimshøyde</td>
      <td>høyde til skjæringen mellom ytterveggens ytre flate og takflaten. Der taket er forsynt med et takoppbygg eller parapet som stikker mer enn 0,3 m opp over takflaten, regnes høyden til toppen av takoppbygget/parapetet. Måles i forhold til ferdig planert terrengs gjennomsnittsnivå rundt bygningen (TEK § 6-2)</td>
      <td></td>
    </tr>
    <tr>
      <td>mønehøyde</td>
      <td>høyde til skjæringen mellom to skrå takflater. Måles i forhold til ferdig planert terrengs gjennomsnittsnivå rundt bygningen  (TEK § 6-2)</td>
      <td></td>
    </tr>
    <tr>
      <td>terrenghøyde</td>
      <td>terrengets høyde</td>
      <td></td>
    </tr>
    <tr>
      <td>planeringshøyde</td>
      <td>høyden av ferdig planert terreng</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Høydereferansesystem

**Definisjon:** referanseflate som er utgangspunktet for høyde. Det skal alltid brukes NN2000 for reguleringplanforslag.

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
      <td>NN2000</td>
      <td>Norsk Null av 2000.
Nytt felles nordisk vertikalt datum, basert på Normaal Amsterdals Peil.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Terrengreferanse

**Definisjon:** kodeliste som angir type terrengoverflate som er utgangspunkt for å angi bygningers høyde

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
      <td>ferdigPlanertTerreng</td>
      <td>gjennomsnittlig nivå av ferdig planert terreng</td>
      <td></td>
    </tr>
    <tr>
      <td>gatenivå</td>
      <td>gatas gjennomsnittsnivå</td>
      <td></td>
    </tr>
    <tr>
      <td>eksistrendeTerreng</td>
      <td>gjennomsnittlig nivå av terreng som ikke er mekanisk behandlet</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» RpJuridiskPunktType

**Definisjon:** kodeliste for type juridisk punkt i reguleringsplan.

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
      <td>Veistengning/fysisk kjøresperre</td>
      <td>Regulert vegstenging</td>
      <td></td>
    </tr>
    <tr>
      <td>Stenging av avkjørsel</td>
      <td>Regulert stengt avkjørsel</td>
      <td></td>
    </tr>
    <tr>
      <td>Avkjørsel - både inn og utkjøring</td>
      <td>Regulert avkjørsel - både inn og utkjøring</td>
      <td></td>
    </tr>
    <tr>
      <td>Avkjørsel - kun innkjøring</td>
      <td>Regulert avkjørsel - kun innkjøring</td>
      <td></td>
    </tr>
    <tr>
      <td>Avkjørsel - kun utkjøring</td>
      <td>Regulert avkjørsel - kun utkjøring</td>
      <td></td>
    </tr>
    <tr>
      <td>Brukar</td>
      <td>Regulert brukar</td>
      <td></td>
    </tr>
    <tr>
      <td>Tunnelåpning</td>
      <td>Regulert tunnelåpning</td>
      <td></td>
    </tr>
    <tr>
      <td>Eksisterende tre som skal bevares</td>
      <td>Regulert bevaring av eksisterende tre</td>
      <td></td>
    </tr>
    <tr>
      <td>Regulert nytt tre</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Regulert møneretning</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» RpJuridiskLinjeType

**Definisjon:** kodeliste for type juridisk linje i reguleringsplan.

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
      <td>Regulert tomtegrense</td>
      <td>Regulert eiendomsgrense</td>
      <td></td>
    </tr>
    <tr>
      <td>Eiendomsgrense som skal oppheves</td>
      <td>Eiendomsgrense som oppheves ved vedtak av plan</td>
      <td></td>
    </tr>
    <tr>
      <td>Bygg, kulturminner, mm. som skal bevares</td>
      <td>Bygg som skal bevares (kun bevaringsområder)</td>
      <td></td>
    </tr>
    <tr>
      <td>Byggegrense</td>
      <td>grense mellom arealer som kan bebygges og ikke kan bebygges.</td>
      <td></td>
    </tr>
    <tr>
      <td>Planlagt bebyggelse</td>
      <td>Omriss av planlagt bebyggelse</td>
      <td></td>
    </tr>
    <tr>
      <td>Bebyggelse som inngår i planen</td>
      <td>Omriss av eksisterende bebyggelse som inngår i planen</td>
      <td></td>
    </tr>
    <tr>
      <td>Bebyggelse som forutsettes fjernet</td>
      <td>Omriss av bebyggelse som forutsettes fjernet</td>
      <td></td>
    </tr>
    <tr>
      <td>Regulert senterlinje</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Frisiktlinje</td>
      <td>grenselinje for område som skal ha frisikt ved kjøring mot vegkryss
Lengden av frisiktlinjen er avhengig av tillatt hastighet og vegkrysstype</td>
      <td></td>
    </tr>
    <tr>
      <td>Regulert kant kjørebane</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Regulert kjørefelt</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Regulert parkeringsfelt</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Regulert fotgjengerfelt</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Regulert støyskjerm</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Regulert støttemur</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Sikringsgjerde</td>
      <td>Regulert sikringsgjerde</td>
      <td></td>
    </tr>
    <tr>
      <td>Bru</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Tunnel</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Måle- og avstandslinje</td>
      <td>linje som viser fastsatt avstand eller radius</td>
      <td></td>
    </tr>
    <tr>
      <td>Strandlinje sjø</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Strandlinje vassdrag</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Midtlinje vassdrag</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>Markagrense</td>
      <td>Grense for område som omfattes av lov om naturområder i Oslo og nærliggende kommuner (markaloven).</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» PåskriftType

**Definisjon:** kode for hva en påskrift på plankartet omhandler

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
      <td>feltkode</td>
      <td>Feltkode, dvs. navn på et kartobjekt (formålOmråde, hensynsSone, bestemmelseOmråde, osv.)</td>
      <td></td>
    </tr>
    <tr>
      <td>areal</td>
      <td>Arealet av delflaten som påskriften refererer til</td>
      <td></td>
    </tr>
    <tr>
      <td>utnytting</td>
      <td>Utnyttingsgrad for formålsområde.</td>
      <td></td>
    </tr>
    <tr>
      <td>målsetting</td>
      <td>Målsatte avstander i kartet.
Referer til avstandslinje med måltall  (juridisk linje 1259)</td>
      <td></td>
    </tr>
    <tr>
      <td>radius</td>
      <td>Radius på sirkelbue.
Brukes på senterlinje for veg og jernbane.</td>
      <td></td>
    </tr>
    <tr>
      <td>kotehøyde</td>
      <td>Høyde over havet.</td>
      <td></td>
    </tr>
  </tbody>
</table>
