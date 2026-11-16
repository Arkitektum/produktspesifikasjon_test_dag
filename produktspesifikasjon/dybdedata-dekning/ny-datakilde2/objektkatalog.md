### Datamodell

**Kilde:** [SOSI UML XMI-fil](https://sosi.geonorge.no/svn/SOSI/SOSI%20Del%203/FKB/Havnedata-2021.xml)

#### Oversikt

<a href="ny-datakilde2_feature_catalogue_overview.png" title="Klikk for stor visning"><img src="ny-datakilde2_feature_catalogue_overview.png" alt="Datamodell Ny datakilde2 - oversikt" style="max-width: 100%; height: auto;" /></a>

#### Pakke: Fellesegenskaper og abstrakte objekttyper

<a href="ny-datakilde2_feature_catalogue_Fellesegenskaper_og_abstrakte_objekttyper.png" title="Klikk for stor visning"><img src="ny-datakilde2_feature_catalogue_Fellesegenskaper_og_abstrakte_objekttyper.png" alt="Datamodell Ny datakilde2 - Fellesegenskaper og abstrakte objekttyper" style="max-width: 100%; height: auto;" /></a>

#### Pakke: Havnedata 2.0

<a href="ny-datakilde2_feature_catalogue_Havnedata_2_0.png" title="Klikk for stor visning"><img src="ny-datakilde2_feature_catalogue_Havnedata_2_0.png" alt="Datamodell Ny datakilde2 - Havnedata 2.0" style="max-width: 100%; height: auto;" /></a>

#### Pakke: Reguleringer

<a href="ny-datakilde2_feature_catalogue_Reguleringer.png" title="Klikk for stor visning"><img src="ny-datakilde2_feature_catalogue_Reguleringer.png" alt="Datamodell Ny datakilde2 - Reguleringer" style="max-width: 100%; height: auto;" /></a>

#### Komplett diagram

<a href="ny-datakilde2_feature_catalogue.png" title="Klikk for stor visning"><img src="ny-datakilde2_feature_catalogue.png" alt="Datamodell Ny datakilde2" style="max-width: 100%; height: auto;" /></a>

#### Kran

Innretning for å løfte eller flytte tunge gjenstander, og hører til på kaien/havnen.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>energikilde</td>
      <td>Kodeliste for å spesifisere energikilden til kranen.</td>
      <td><a href="#kodeliste-energikilde">Energikilde</a><br />(kodeliste)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kranspesifikasjon</td>
      <td>Spesifikasjon for kranen.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>krantype</td>
      <td>Krantype.</td>
      <td><a href="#kodeliste-krantype">Krantype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>maksbelastning</td>
      <td>Maks løfteevne for krana angitt i tonn (ved liten arm).</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>maksbelastning<wbr />Rekkevidde</td>
      <td>Maks løfteevne for krana ved maksimal arm/rekkevidde angitt i antall tonn.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>mobilitet</td>
      <td>Egenskap for å angi om en krane er fastmontert eller flyttbar (mobil).<br />Fastmontert krane står i et fast punkt på kaia, mens mobile kraner kan flyttes. Skinnegående kraner eller andre semi-mobile kraner angis som mobile.<br />For mobile kraner registreres punktet som en skjønnsmessig representativ koordinat for krana.</td>
      <td>Boolean</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Posisjon</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>rekkevidde</td>
      <td>Rekkevidden til kranen, ut fra kaifronten, i antall meter.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra ObjektId</th>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unikt løpenummer for identifisering av det enkelte objekt på kaien, i form av nummer/tekst.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
ObjektId

#### HavneanleggGrense

Avgrensning av havneanlegg.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>grense</td>
      <td>Forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperPåkrevd

#### VAuttak

Tilkoblingspunkt for vann på kaia.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kapasitet</td>
      <td>Kapasitet til fylling av vann angitt i antall m3/time.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kumnummer</td>
      <td>ID-merking av kummer. Kan tas fra havnas eget merkesystem eller kommunens SID-nr.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Posisjon</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>tilgangstype</td>
      <td>Kodeliste for å spesifisere hvem som har mulighet til å benytte uttaket.</td>
      <td><a href="#kodeliste-tilgangstype">Tilgangstype</a><br />(kodeliste)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>tilkoblingsdimensjon</td>
      <td>Størrelse/dimensjon på rørene som skal kobles sammen.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>VAuttakstype</td>
      <td>Beskrivelse av hva slags uttakstype som kan gjøres.</td>
      <td><a href="#kodeliste-vauttakstype">VAuttakstype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra ObjektId</th>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unikt løpenummer for identifisering av det enkelte objekt på kaien, i form av nummer/tekst.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
ObjektId

#### Havneanlegg

Med havneanlegg menes arealer, bygninger, innretninger og annen infrastruktur som brukes i havnevirksomhet eller havneformål. Herunder: kaier, terminalbygninger, laste-, losse- og omlastningsinnretninger og lager- og administrasjonsbygninger.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>eier</td>
      <td>Eier av havneanlegget.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>eierskap</td>
      <td>Felt for å angi type eierskap.</td>
      <td><a href="#kodeliste-eierskap">Eierskap</a><br />(kodeliste)</td>
      <td>1..*</td>
    </tr>
    <tr>
      <td>forvaltes<wbr />Av</td>
      <td>Felt for å angi hvem havneanlegget forvaltes av.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPSHavneanlegg</td>
      <td>Egenskaper spesifikke for ISPSHavneanlegg.</td>
      <td>ISPSHavneanlegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- kontaktinformasjon<wbr />PFSO</td>
      <td>Kontaktinformasjon til PFSP eller assisterende PFSO på det aktuelle ISPS-området.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- port<wbr />Facility<wbr />Nr<wbr />IMO</td>
      <td>Lokasjonskode for ISPS-området. Består av UNLOCODE, samt en 4-siffret tallkode.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- sikkerhetsbarriere</td>
      <td>Attributt for å spesifisere om et havnesikkerhetsområde ikke har inngjerding eller annen form for sikkerhetsbarriere.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- sikringstype</td>
      <td>Beskriver sikring/tilgang til havnesikkerhetsområdet.</td>
      <td><a href="#kodeliste-sikringstype">Sikringstype</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- status<wbr />Godkjenning</td>
      <td>Felt for å angi status på ISPS godkjenning.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>område</td>
      <td>Polygon som viser geografisk utstrekning.</td>
      <td>Flate</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Opsjonelt representasjonspunkt for området.</td>
      <td>Punkt</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
HavneanleggId

**Assosiasjoner**
HavneanleggGrense – rolle: avgrensning – kardinalitet: 0..*

#### Flytedokk

En flytedokk eller våtdokk er en flytende plattform for å heve skip opp av sjøen når det skal gjøres vedlikehold eller reperasjoner av skip.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>løftekapasitet</td>
      <td>Maksimal løftekapasitet, angitt i tonn.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>maks<wbr />Fartøy<wbr />Bredde</td>
      <td>Maksimal bredde på fartøyet som dokken kan romme. Angis i meter.</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>maks<wbr />Fartøy<wbr />Dyptgående</td>
      <td>Maksimal dyptgående på fartøyet som dokken kan romme. Angis i meter.</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>maks<wbr />Fartøy<wbr />Lengde</td>
      <td>Maksimal lengde på fartøyet som dokken kan romme. Angis i meter.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Navn på flytedokken.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>område</td>
      <td>Polygon som viser geografisk utstrekning.</td>
      <td>Flate</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Opsjonelt representasjonspunkt for området.</td>
      <td>Punkt</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
HavneanleggId

**Assosiasjoner**
FlytedokkGrense – rolle: avgrensning – kardinalitet: 0..*

#### Toalett

Offentlig toalett.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Posisjon</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra ObjektId</th>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unikt løpenummer for identifisering av det enkelte objekt på kaien, i form av nummer/tekst.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
ObjektId

#### FlytedokkGrense

Avgrensning av Flytedokk.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>grense</td>
      <td>Forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperPåkrevd

#### Fender

Beskytter/demper for bevegelse mellom båt og kai. Monteres ofte fast på kaikanten.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>antall</td>
      <td>Oppgi antall fendere. Benyttes ved gruppering av fendere.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>fendergruppering</td>
      <td>Kurve geometri som brukes ved gruppering av fendere.<br />Geometrien skal følge kaifront der hvor det er mange like fendere. Antall fendere oppgis i antall-felt, og avstand spesifiseres i informasjonsfeltet.</td>
      <td>Kurve</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>fenderorientering</td>
      <td>Retning/orientering på fenderen.</td>
      <td><a href="#kodeliste-fenderorientering">Fenderorientering</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>fenderspesifikasjon</td>
      <td>Egenskap for å spesifisere fender. Fenderen kan beskrives med mål, for eksempel bredde, høyde, diameter etc.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>fendertype</td>
      <td>Fendertype</td>
      <td><a href="#kodeliste-fendertype">Fendertype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>høyde<wbr />Sjøkartnull</td>
      <td>Angitt høyde i meter over vannet. Egenskapen høyde angis i forhold til sjøkartnull (dvs. høyder over lokal LAT-verdi) dersom ikke annet er angitt.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Posisjon</td>
      <td>Punkt</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra ObjektId</th>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unikt løpenummer for identifisering av det enkelte objekt på kaien, i form av nummer/tekst.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
ObjektId

#### LastbegrensningsområdeGrense

Avgrensning av lastbegrensningsområde.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>grense</td>
      <td>Forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperPåkrevd

#### Avfallspunkt

punkt for å kaste avfall

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>avfallsplan</td>
      <td>Henvisning til avfallsplan som gjør rede for planlagt håndtering av avfall.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>avfallstype</td>
      <td>Avfallstype</td>
      <td><a href="#kodeliste-avfallstype">Avfallstype</a><br />(kodeliste)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>beholdertype</td>
      <td>Beholdertype</td>
      <td><a href="#kodeliste-beholdertype">Beholdertype</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>mobilitet</td>
      <td>Egenskap for å anngi om avfallspunktet er fast montert eller flyttbart ( i form av en bil eller lignende).<br /><br />For mobile tilkoblingspunkt er det vanskelig/meningsløst å stedfeste punktet nøyaktig. Punktet plasseres da på et passelig representativt punkt og gis en kvalitetskode som angir stor usikkerhet i innmåling.</td>
      <td>Boolean</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Posisjon</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>tilgangstype</td>
      <td>Kodeliste for å spesifisere hvem som har mulighet til å benytte avfallspunktet.</td>
      <td><a href="#kodeliste-tilgangstype">Tilgangstype</a><br />(kodeliste)</td>
      <td>0..*</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra ObjektId</th>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unikt løpenummer for identifisering av det enkelte objekt på kaien, i form av nummer/tekst.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
ObjektId

#### Kaiområde

Kaiområde er området direkte innenfor kaifronten som tilhører den samme kaien.<br />Kaiområde avgrenses av KaiområdeGrense. Kaifront brukes ikke som avgrensning til kaiområde, men ligger som et eget objekt.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>kaidekketype</td>
      <td>Beskrivelse av materialbruk på dekke av kaia (betong, asfalt, tre e.l.)</td>
      <td><a href="#kodeliste-kaidekketype">Kaidekketype</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kaitype</td>
      <td>Angivelse av kaitype.</td>
      <td><a href="#kodeliste-kaitype">Kaitype</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>område</td>
      <td>Område</td>
      <td>Flate</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Opsjonelt representasjonspunkt for området.</td>
      <td>Punkt</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
KaiId

**Assosiasjoner**
KaiområdeGrense – rolle: avgrensning – kardinalitet: 0..*

#### Fortøyningsinnretning

Fortøyningsinnretning som tilhører kaia.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>fortøyningstype</td>
      <td>Fortøyningstype</td>
      <td><a href="#kodeliste-fortøyningstype">Fortøyningstype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>høyde<wbr />Sjøkartnull</td>
      <td>Angitt høyde i meter over vannet. Egenskapen høyde angis i forhold til sjøkartnull (dvs. høyder over lokal LAT-verdi) dersom ikke annet er angitt.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>maksbelastning</td>
      <td>Beskrivelse av maks belastning for pullerten i antall tonn</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Posisjon</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>sertifiseringsdato</td>
      <td>Dato for forrige sertifisering.</td>
      <td>Date</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spesifikasjon</td>
      <td>Egenskap for å spesifisere fortøyningsinnretning.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>tillatt<wbr />Fortøyningsvinkel<wbr />Grunnriss</td>
      <td>Tillatt område for fortøyning sett i grunnriss. Eksempel: +/-90°.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>tillatt<wbr />Fortøyningsvinkel<wbr />Oppriss</td>
      <td>Tillatt område for fortøyning sett i oppriss. Eksempel: +75°/-15°.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra ObjektId</th>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unikt løpenummer for identifisering av det enkelte objekt på kaien, i form av nummer/tekst.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
ObjektId

#### Havnegjerde

Gjerde eller annen barriere. Følger ofte Havnesikkerhetsområde, men brukes ikke som avgrensning. Havnesikkerhetsområde avgrenses av HavnesikkerhetsområdeGrense.<br />Havnegjerde vil også ofte være kartlagt i FKB-BygnAnlegg som AnnetGjerde, mur e.l. I så fall bør disse objektene ha sammenfallende geometri.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>periode</td>
      <td>Periode havnegjerdet er satt opp. Brukes i tilfeller der havnegjerde er kun satt opp i visse tidsrom eller deler av året.  Attributt trengs ikke benyttes ved permanent gjerde.</td>
      <td>Periode<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- mnd<wbr />Fra</td>
      <td>Måned fra.</td>
      <td><a href="#kodeliste-måned">Måned</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- mnd<wbr />Til</td>
      <td>Måned til.</td>
      <td><a href="#kodeliste-måned">Måned</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>senterlinje</td>
      <td>Forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
HavneanleggId

#### Tørrdokk

Et basseng stort nok til at skip kan seile ut og inn. Bunnen ligger lavere enn havnivået og innløpet kan lukkes med porter. Vann kan pumpes ut, slik skip kan stå tørt, for vedlikehold og reperasjon.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>løftekapasitet</td>
      <td>Maksimal løftekapasitet, angitt i tonn.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>maks<wbr />Fartøy<wbr />Bredde</td>
      <td>Maksimal bredde på fartøyet som dokken kan romme. Angis i meter.</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>maks<wbr />Fartøy<wbr />Dyptgående</td>
      <td>Maksimal dyptgående på fartøyet som dokken kan romme. Angis i meter.</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>maks<wbr />Fartøy<wbr />Lengde</td>
      <td>Maksimal lengde på fartøyet som dokken kan romme. Angis i meter.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Navn på tørrdokken.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>område</td>
      <td>Polygon som viser geografisk utstrekning.</td>
      <td>Flate</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Opsjonelt representasjonspunkt for området.</td>
      <td>Punkt</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
HavneanleggId

**Assosiasjoner**
TørrdokkGrense – rolle: avgrensning – kardinalitet: 0..*

#### KaiområdeGrense

Avgrensning av kaiområde.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>grense</td>
      <td>Forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperPåkrevd

#### HavnegjerdeInngang

Inngang, åpning eller innkjørsel til området som er avsperret av Havnegjerde.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>avsperringstype</td>
      <td>Kodeliste for å angi type avsperring for inngangen.</td>
      <td><a href="#kodeliste-avsperringstype">Avsperringstype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>periode</td>
      <td>Periode havnegjerdet og/eller havnegjerdeInngang er satt opp. Brukes i tilfeller der havnegjerde er kun satt opp i visse tidsrom eller deler av året.  Attributt trengs ikke benyttes ved permanent gjerde.</td>
      <td>Periode<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- mnd<wbr />Fra</td>
      <td>Måned fra.</td>
      <td><a href="#kodeliste-måned">Måned</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- mnd<wbr />Til</td>
      <td>Måned til.</td>
      <td><a href="#kodeliste-måned">Måned</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>senterlinje</td>
      <td>Forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>åpningstype</td>
      <td>Kodeliste for å spesifisere åpningsmekanisme av port, bom eller annet som avsperrer havnesikkerhetsområde.</td>
      <td><a href="#kodeliste-åpningstype">Åpningstype</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
HavneanleggId

#### ForvaltningsområdeGrense

Avgrensning av forvaltningsområde.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>grense</td>
      <td>Forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperPåkrevd

#### SlippGrense

Avgrensning av Slipp.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>grense</td>
      <td>forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperPåkrevd

#### TørrdokkGrense

Avgrensning av Tørrdokk.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>grense</td>
      <td>forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperPåkrevd

#### HavneområdeGrense

Avgrensning av havneområde.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>grense</td>
      <td>Forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperPåkrevd

#### Havneområde

Havn er et avgrenset område som inneholder kai/kaier tilknyttet land- og sjøarealer som er tilrettelagt for overføring av gods, personer eller lignende mellom land og sjø.<br />Havneområde kjennetegnes ved at de har en UNLOCODE tilknyttet seg, og innenfor området må det være minst én kai og én kaifront.<br />Havneområdet kan inneholde mange havneanlegg, mange kaier og andre objekter.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>forvaltes<wbr />Av</td>
      <td>Felt for å angi hvem som forvalter eller administrerer havneområdet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>område</td>
      <td>Polygon som viser geografisk utstrekning</td>
      <td>Flate</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Opsjonelt representasjonspunkt.</td>
      <td>Punkt</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
HavnId

**Assosiasjoner**
HavneområdeGrense – rolle: avgrensning – kardinalitet: 0..*

#### Forvaltningsområde

Areal som viser utstrekningen på det område en kommune eller en kommunal/interkommunal havneadministrasjonen har ansvaret for. Dette området er ofte sammenfallende med kommunens sjøområde, som er det område hvor kommunen har planmyndighet etter plan- og bygningsloven med unntak av hoved- og biled (Hoved- og biled forvaltes av Kystverket).

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>forvaltes<wbr />Av</td>
      <td>Felt for å angi hvem som forvalter området. Vanligvis kommune, IKS eller havneadministrasjon på vegne av kommune.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>område</td>
      <td>Polygon som viser geografisk utstrekning.</td>
      <td>Flate</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Opsjonelt representasjonspunkt for området.</td>
      <td>Punkt</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
HavnId

**Assosiasjoner**
ForvaltningsområdeGrense – rolle: avgrensning – kardinalitet: 0..*

#### Beredskapspunkt

Punkt på kaia der det er plassert utstyr for beredskap/sikkerhet.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>beredskapstype</td>
      <td>Beredskapstype</td>
      <td><a href="#kodeliste-beredskapstype">Beredskapstype</a><br />(kodeliste)</td>
      <td>1..*</td>
    </tr>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Posisjon</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>spesifikasjon</td>
      <td>Egenskap for å spesifisere beredskapstype.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra ObjektId</th>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unikt løpenummer for identifisering av det enkelte objekt på kaien, i form av nummer/tekst.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
ObjektId

#### Kaifront

Kaifront er den ytterste delen av kaien, som avgrenser sjøen fra land, hvor fartøy kan ligge fortøyd langs.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>høyde<wbr />Sjøkartnull</td>
      <td>Angitt høyde på kaien i meter over vannet. Egenskapen høyde angis i forhold til sjøkartnull (dvs. høyder over lokal LAT-verdi) dersom ikke annet er angitt.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kaifronttype</td>
      <td>Beskriver type konstruksjon kaifronten har mot sjøen.</td>
      <td><a href="#kodeliste-kaifronttype">Kaifronttype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kaitype</td>
      <td>Type kai</td>
      <td><a href="#kodeliste-kaitype">Kaitype</a><br />(kodeliste)</td>
      <td>1..*</td>
    </tr>
    <tr>
      <td>lengde</td>
      <td>Angitt lengde på kaifronten i antall meter. Kailengden måles opp på den delen av kaifronten som egner seg for anløp av skip. Lengde kan også beregnes ut fra lengden på geometrien.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>senterlinje</td>
      <td>Forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra ObjektId</th>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unikt løpenummer for identifisering av det enkelte objekt på kaien, i form av nummer/tekst.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
ObjektId

#### Havnesensor

Sensor som måler, samler inn data eller registrerer annet i tilknytning til havnen.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unik identisfisering av det enkelte objekt på kaia i form av URL, nummer, navn eller annet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Posisjon</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>sensortype</td>
      <td>Type sensor.</td>
      <td><a href="#kodeliste-sensortype">Sensortype</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
HavnId

#### Slipp

Skinnegående bane eller et forseggjort opptrekk som fartøy kan hales opp ved landsetting, fra flytende posisjon og opp på tørt land. Skråplanet går vanligvis ut og ned i vannet.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>høyde<wbr />Sjøkartnull</td>
      <td>Angitt høyde på høyeste del av slippen, i meter over vannet. Egenskapen høyde angis i forhold til sjøkartnull (dvs. høyder over lokal LAT-verdi) dersom ikke annet er angitt.</td>
      <td>Real</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kaidekketype</td>
      <td>Beskrivelse av materialebruk på dekket av slippen.</td>
      <td><a href="#kodeliste-kaidekketype">Kaidekketype</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kran<wbr />Kapasitet</td>
      <td>Kapasitet til kran tilknyttet slipp, angitt i tonn.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>maks<wbr />Bredde<wbr />Fartøy</td>
      <td>Maksimal bredde på fartøyet som slippen kan ta. Angis i meter.</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>maks<wbr />Dyptgående<wbr />Fartøy</td>
      <td>Maksimal dyptgående på fartøyet som slippen kan ta. Angis i meter.</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>maks<wbr />Lengde<wbr />Fartøy</td>
      <td>Maksimal lengde på fartøy som slippen kan ta. Angis i meter.</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Navn på slippen.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>område</td>
      <td>Polygon som viser geografisk utstrekning.</td>
      <td>Flate</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Opsjonelt representasjonspunkt for området.</td>
      <td>Punkt</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>slipp<wbr />Kapasitet</td>
      <td>Løftekapasitet til slippen, angitt i tonn.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spesifikasjon</td>
      <td>Attributt for å spesifisere opptrekksmekanisme (vinsj, skinner el.) eller annen relevant informasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>tilgangstype</td>
      <td>Kodeliste for å spesifisere hvem som har mulighet til å benytte slippen.</td>
      <td><a href="#kodeliste-tilgangstype">Tilgangstype</a><br />(kodeliste)</td>
      <td>0..*</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
KaiId

**Assosiasjoner**
SlippGrense – rolle: avgrensning – kardinalitet: 0..*

#### Lastbegrensningsområde

Område i havnen eller på kai som har begrensinger for hva det tåler av belastning.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>akseltrykk</td>
      <td>Det trykk som må bæres av én aksel på en vogn eller kjøretøy.<br />Øvre grense for akseltrykk. Måles i tonn (t).</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>bruksklassetype</td>
      <td>Bruksklasse</td>
      <td><a href="#kodeliste-bruksklassetype">Bruksklassetype</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kaidekketype</td>
      <td>Kaidekke</td>
      <td><a href="#kodeliste-kaidekketype">Kaidekketype</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>last<wbr />Id</td>
      <td>Tall eller tekst havnen bruker for å identifisere et lastbegrensningsområde.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>lastreferanse</td>
      <td>Referanse til originaldokument, tegning e.l. som inneholder informasjon om lastebegrensing.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>minste<wbr />Avstand<wbr />Punktlast</td>
      <td>Hvor tett to punktlaster kan stå for å ikke overbelaste kaien. Henger sammen med egenskapen punktlast. Måles i meter (m).</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>område</td>
      <td>Område</td>
      <td>Flate</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Opsjonelt representasjonspunkt for området.</td>
      <td>Punkt</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>punktlast</td>
      <td>Vekten av last fordelt i et punkt. Øvre grense for maksimal vekt av en punktlast. Måles i tonn (t).</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>vektbegrensning</td>
      <td>Vekten av jevnt fordelt last over et område. Øvre grense for jevnt fordelt last. Måles i antall tonn pr. kvadratmeter (t/m2).</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
KaiId

**Assosiasjoner**
LastbegrensningsområdeGrense – rolle: avgrensning – kardinalitet: 0..*

#### Kamera

Kamera tilknyttet havnen.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unik identisfisering av det enkelte objekt på kaia i form av URL, nummer, navn eller annet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Posisjon</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
HavnId

#### Drivstofftilkobling

Tilkoblingspunkt for drivstoff på kaia.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>drivstofftype</td>
      <td>Type drivstoff.</td>
      <td><a href="#kodeliste-drivstofftype">Drivstofftype</a><br />(kodeliste)</td>
      <td>1..*</td>
    </tr>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kapasitet</td>
      <td>Kapasitet til fylling av drivstoff angitt i antall m3/time.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>mobilitet</td>
      <td>Egenskap for å anngi om drivstoffpunktet er fast montert eller flyttbart (mobilt drivstoffpunkt i form av en tankbil eller lignende).<br /><br />For mobile tilkoblingspunkt er det vanskelig/meningsløst å stedfeste punktet nøyaktig. Punktet plasseres da på et passelig representativt punkt og gis en kvalitetskode som angir stor usikkerhet i innmåling.</td>
      <td>Boolean</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Posisjon</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>tilgangstype</td>
      <td>Kodeliste for å spesifisere hvem som har mulighet til å benytte punktet.</td>
      <td><a href="#kodeliste-tilgangstype">Tilgangstype</a><br />(kodeliste)</td>
      <td>0..*</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra ObjektId</th>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unikt løpenummer for identifisering av det enkelte objekt på kaien, i form av nummer/tekst.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
ObjektId

#### Tømmestasjon

Tømmestasjon eller punkt for tømming av væske (avløpsvann, septik eller tilsvarende).

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>avløpstype</td>
      <td>Beskrivelse av hva slags tømming/avløpstype som er tilgjengelig.</td>
      <td><a href="#kodeliste-avløpstype">Avløpstype</a><br />(kodeliste)</td>
      <td>1..*</td>
    </tr>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kapasitet</td>
      <td>Kapasitet til tømming, angitt i antall m3/time.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kumnummer</td>
      <td>ID-merking av kummer. Kan tas fra havnas eget merkesystem eller kommunens SID-nr.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>mobilitet</td>
      <td>Egenskap for å anngi om tømmestasjonen er fast montert eller flyttbart (i form av en tankbil eller lignende).<br /><br />For mobile tilkoblingspunkt er det vanskelig/meningsløst å stedfeste punktet nøyaktig. Punktet plasseres da på et passelig representativt punkt og gis en kvalitetskode som angir stor usikkerhet i innmåling.</td>
      <td>Boolean</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Posisjon</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>tilgangstype</td>
      <td>Kodeliste for å spesifisere hvem som har mulighet til å benytte tømmestasjonen.</td>
      <td><a href="#kodeliste-tilgangstype">Tilgangstype</a><br />(kodeliste)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>tilkoblingsdimensjon</td>
      <td>Størrelse/dimensjon på rørene som skal kobles sammen.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra ObjektId</th>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unikt løpenummer for identifisering av det enkelte objekt på kaien, i form av nummer/tekst.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
ObjektId

#### ELkobling

Tilkoblingspunkt for strøm på kaia.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>ELanleggstype</td>
      <td>Beskrivelse av hva slags type strømtilkobling som kan gjøres.</td>
      <td><a href="#kodeliste-elanleggstype">ELanleggstype</a><br />(kodeliste)</td>
      <td>1..*</td>
    </tr>
    <tr>
      <td>ELkoblinger</td>
      <td>Spesifikasjon av de ulike kombinasjonene EL-koblingspunkt som finnes.</td>
      <td>ELkobling<wbr />Egenskaper<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- effekt</td>
      <td>Watt. Arbeid pr. sekund.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- faser</td>
      <td>Betegnelse på de enkelte polene eller lederne i et vekselstrømsystem.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- frekvens</td>
      <td>Hvor mange ganger en elektrisk spenning veksler i løpet av ett sekund. Måles i Hz.</td>
      <td><a href="#kodeliste-frekvens">Frekvens</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- kontakt<wbr />Id</td>
      <td>Id-nummer eller annen beskrivelse som spesifiserer hvilken type kontakt.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- sikringstørrelse</td>
      <td>Strømstyrke, oppgis i ampere, SI-enheten for elektrisk strøm. Strømstyrke er lik ladning som passerer et tverrsnitt av en leder pr. sekund.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- spenning</td>
      <td>Volt. Elektrisk spenning.</td>
      <td><a href="#kodeliste-spenning">Spenning</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>høydereferanse</td>
      <td>Høydereferanse til kartobjektet.</td>
      <td><a href="#kodeliste-høydereferanse">Høydereferanse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Posisjon</td>
      <td>Punkt</td>
      <td>1</td>
    </tr>
    <tr>
      <td>rekkevidde<wbr />Ladeanlegg</td>
      <td>Attributt som benyttes ved ladeannlegg, for å spesifisere lengde på kabeltrommel som er tilgjengelig. Oppgis i meter.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Beskriver status til et objekt.</td>
      <td><a href="#kodeliste-status">Status</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>tilgangstype</td>
      <td>Kodeliste for å spesifisere hvem som har mulighet til å benytte punktet.</td>
      <td><a href="#kodeliste-tilgangstype">Tilgangstype</a><br />(kodeliste)</td>
      <td>0..*</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra ObjektId</th>
    </tr>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unikt løpenummer for identifisering av det enkelte objekt på kaien, i form av nummer/tekst.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
ObjektId

#### HavneanleggId (abstrakt)

Abstrakt objekt som holder egenskaper for unik identifisering av et havneanlegg. Egenskapene arves ned til øvrige objektklasser i Havnedata.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
HavnId

#### FellesegenskaperOpsjonell (abstrakt)

abstrakt objekt som bærer en felles egenskaper som brukes på alle objekttyper i FKB.<br />Opsjonelle egenskaper.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperPåkrevd

#### FellesegenskaperPåkrevd (abstrakt)

abstrakt objekt som bærer en felles egenskaper som brukes på alle objekttyper i FKB.<br />Påkrevde egenskaper.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

#### HavnId (abstrakt)

Abstrakt objekt som holder egenskaper for unik identifisering av en havn. Egenskapene arves ned til øvrige objektklasser i Havnedata.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperOpsjonell

#### KaiId (abstrakt)

Abstrakt objekt som holder egenskaper for unik identifisering av en kai. Egenskapene arves ned til øvrige objektklasser i Havnedata.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
HavneanleggId

#### ObjektId (abstrakt)

Abstrakt objekt som holder egenskaper for unik identifisering av objekt på kaien.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>objekt<wbr />Løpenummer</td>
      <td>Unikt løpenummer for identifisering av det enkelte objekt på kaien, i form av nummer/tekst.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra KaiId</th>
    </tr>
    <tr>
      <td>kai<wbr />Id</td>
      <td>Unik identifisering av den enkelte kai.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kai<wbr />Id<wbr />Intern</td>
      <td>Havnens interne egendefinerte nummering av kaier.<br />Nummerering varierer fra havn til havn, noen bruker utelukkende tall eller bokstaver, mens andre bruker en kombinasjon.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kainavn</td>
      <td>Navn på kaien. Det samme kainavnet brukes på alle kaifronter og kaiområder som regnes å tilhøre samme kai. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavneanleggId</th>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Id</td>
      <td>Unik identifisering av det enkelte havneanlegg.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>havneanlegg<wbr />Navn</td>
      <td>Navn på havneanlegg. Navn bør stemme overens med SafeSeaNet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>ISPS</td>
      <td>Boolsk verdi (JA/NEI) om angir om havneanlegget er et ISPS Havneanlegg.</td>
      <td>Boolean</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra HavnId</th>
    </tr>
    <tr>
      <td>havn</td>
      <td>Stedsnavn på havnen som har blitt tildelt en UNLOCODE. Navnet må samsvare med UNLOCODE.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>UNLOCODE</td>
      <td>Lokaliseringskode fra UNLOCODE-systemet som identifiserer et havneområde. Koden består av 5 bokstaver: de to første bokstavene angir landskode, mens de tre siste identifiserer havnen. Eks: NOSVG (Stavanger).<br />Se liste med lovlige kodeverdier her: <a href="https://service.unece.org/trade/locode/no.htm">https://service.unece.org/trade/locode/no.htm</a></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
KaiId

#### Forbudsområde

Område som er omfattet av forbud, som f.eks. ferdselsforbud for vannscooter.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>fastsatt<wbr />Av</td>
      <td>Angir hvem forskriften er fastsatt av.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>forbudstype</td>
      <td>Angir hvilket type forbud som gjelder for området.</td>
      <td><a href="#kodeliste-forbudstype">Forbudstype</a><br />(kodeliste)</td>
      <td>1..*</td>
    </tr>
    <tr>
      <td>forskrift<wbr />Lenke</td>
      <td>Lenke til forskiften på lovdata.no.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>forskrift<wbr />Navn</td>
      <td>Navnet på forskrift som regulerer forbudsområdet. Ved langt navn kan korttittel benyttes.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>gjelder<wbr />For</td>
      <td>Geografisk område som forskriften gjelder for. Står spesifisert i lovteksten, kan være en kommune eller et havneområde.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>gjelder<wbr />For<wbr />Fartøytype</td>
      <td>Kodeliste som spesifiserer hvilken type fartøy som er omfattet av forbudet.</td>
      <td><a href="#kodeliste-fartøytype">Fartøytype</a><br />(kodeliste)</td>
      <td>1..*</td>
    </tr>
    <tr>
      <td>lovhjemmel</td>
      <td>Lov som forbudet eller forskriften har hjemmel i.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>område</td>
      <td>Polygon som viser geografisk utstrekning.</td>
      <td>Flate</td>
      <td>1</td>
    </tr>
    <tr>
      <td>periode<wbr />Gyldig<wbr />Fra</td>
      <td>Periode gyldig fra. Oppgis for forbudsområder som har tidsavgrensning eller gjelder deler av året (f.eks. bare i sommermånedene). Årstall er ikke nødvendig. Dersom årstall ikke oppgis regnes datoen å gjelde hvert år.</td>
      <td>Date</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>periode<wbr />Gyldig<wbr />Til</td>
      <td>Periode gyldig til. Oppgis for forbudsområder som har tidsavgrensning eller gjelder deler av året (f.eks. bare i sommermånedene). Årstall er ikke nødvendig. Dersom årstall ikke oppgis regnes datoen å gjelde hvert år.</td>
      <td>Date</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Opsjonelt representasjonspunkt for området.</td>
      <td>Punkt</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperOpsjonell

**Assosiasjoner**
ForbudsområdeGrense – rolle: avgrensning – kardinalitet: 0..*

#### Fartsrestriksjoner

Område som har restriksjoner knyttet til ferdsel og fart for fartøyer som ferdes på sjøen.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>fastsatt<wbr />Av</td>
      <td>Angir hvem forskriften er fastsatt av.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>forskrift<wbr />Lenke</td>
      <td>Lenke til forskriften på lovdata.no.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>forskrift<wbr />Navn</td>
      <td>Navnet på forskriften. Ved langt navn korttittel benyttes.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>gjelder<wbr />For</td>
      <td>Geografisk område som forskriften gjelder for. Står spesifisert i lovteksten, og er vanligvis en kommune eller havneområde,</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>gjelder<wbr />For<wbr />Fartøytype</td>
      <td>Kodeliste som spesifiserer hvilken type fartøy som er omfattet av forskriften.</td>
      <td><a href="#kodeliste-fartøytype">Fartøytype</a><br />(kodeliste)</td>
      <td>1..*</td>
    </tr>
    <tr>
      <td>hastighet</td>
      <td>Maksimal tillatte hastighet, angitt i knop.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lovhjemmel</td>
      <td>Lov som forskriften har hjemmel i.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>område</td>
      <td>Polygon som viser geografisk utstrekning.</td>
      <td>Flate</td>
      <td>1</td>
    </tr>
    <tr>
      <td>periode<wbr />Gyldig<wbr />Fra</td>
      <td>Periode gyldig fra. Oppgis for fartsrestriksjoner som har tidsavgrensning eller gjelder deler av året (f.eks. bare i sommermånedene). Årstall er ikke nødvendig. Dersom årstall ikke oppgis regnes datoen å gjelde hvert år.</td>
      <td>Date</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>periode<wbr />Gyldig<wbr />Til</td>
      <td>Periode gyldig til. Oppgis for fartsrestriksjoner som har tidsavgrensning eller gjelder deler av året (f.eks. bare i sommermånedene). Årstall er ikke nødvendig. Dersom årstall ikke oppgis regnes datoen å gjelde hvert år.</td>
      <td>Date</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>posisjon</td>
      <td>Opsjonelt representasjonspunkt for området.</td>
      <td>Punkt</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperOpsjonell</th>
    </tr>
    <tr>
      <td>informasjon</td>
      <td>generell opplysning</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>link</td>
      <td>Link i form av URL eller annet til mer informasjon om objektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>oppdateringsdato</td>
      <td>dato for siste endring på objektetdataene.</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperOpsjonell

**Assosiasjoner**
FartsrestriksjonerGrense – rolle: avgrensning – kardinalitet: 0..*

#### ForbudsområdeGrense

Avgrensning av forbudsområde.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>grense</td>
      <td>Forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperPåkrevd

#### FartsrestriksjonerGrense

Avgrensning av Fartsrestriksjoner.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>grense</td>
      <td>Forløp som følger overgang mellom ulike fenomener.</td>
      <td>Kurve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FellesegenskaperPåkrevd</th>
    </tr>
    <tr>
      <td>datafangstdato</td>
      <td>dato når objektet siste gang ble registrert/observert/målt i terrenget</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Unik identifikasjon av objektet.</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>Unik identifikator innenfor navnerommet. For FKB benyttes UUID.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom i form av en URI</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen. Benyttes normalt ikke i FKB.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Stedfestingskvalitet</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode</td>
      <td>Metode for datafangst.<br />Egenskapen beskriver datafangstmetode for grunnrisskoordinater (x,y), eller for både grunnriss og høyde (x,y,z) dersom det ikke er oppgitt noen verdi for datafangstmetodeHøyde.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- datafangstmetode<wbr />Høyde</td>
      <td>Metode brukt for høyderegistrering av posisjon.<br />Det er bare nødvending å angi en verdi for egenskapen dersom datafangstmetode for høyde avviker fra datafangstmetode for grunnriss.</td>
      <td><a href="#kodeliste-datafangstmetode">Datafangstmetode</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- nøyaktighet</td>
      <td>Punktstandardavviket i grunnriss for punkter samt tverravvik for linjer.<br /><br />Merknad:<br />Oppgitt i cm</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- nøyaktighet<wbr />Høyde</td>
      <td>Nøyaktighet for høyden i cm.</td>
      <td>Integer</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- synbarhet</td>
      <td>Hvor godt den kartlagte detalj var synbar ved kartleggingen.</td>
      <td><a href="#kodeliste-synbarhet">Synbarhet</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FellesegenskaperPåkrevd

### Kodelister

#### <a id="kodeliste-energikilde"></a>«CodeList» Energikilde

**Definisjon:** Kodeliste for å spesifisere energikilden til et objekt, f.eks. kran.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/energikilde">https://register.geonorge.no/sosi-kodelister/havnedata/energikilde</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-høydereferanse"></a>«CodeList» Høydereferanse

**Definisjon:** Angivelse av hvor på objektet koordinatregistreringen er utført.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/hoydereferanse">https://register.geonorge.no/sosi-kodelister/havnedata/hoydereferanse</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-krantype"></a>«CodeList» Krantype

**Definisjon:** Angir hvilken type kran.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/krantype">https://register.geonorge.no/sosi-kodelister/havnedata/krantype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-status"></a>«CodeList» Status

**Definisjon:** Angir status til havneobjekt.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/status">https://register.geonorge.no/sosi-kodelister/havnedata/status</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-tilgangstype"></a>«CodeList» Tilgangstype

**Definisjon:** Angir tilgang til havneobjekt.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/tilgangstype">https://register.geonorge.no/sosi-kodelister/havnedata/tilgangstype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-vauttakstype"></a>«CodeList» VAuttakstype

**Definisjon:** Type vanntilkobling som kan gjøres.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/vauttakstype">https://register.geonorge.no/sosi-kodelister/havnedata/vauttakstype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-eierskap"></a>«CodeList» Eierskap

**Definisjon:** Angir type eierskap.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/eierskap">https://register.geonorge.no/sosi-kodelister/havnedata/eierskap</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-sikringstype"></a>«CodeList» Sikringstype

**Definisjon:** Angir sikring til havneobjekt.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/sikringstype">https://register.geonorge.no/sosi-kodelister/havnedata/sikringstype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-fenderorientering"></a>«CodeList» Fenderorientering

**Definisjon:** Angir orientering til fender.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/fenderorientering">https://register.geonorge.no/sosi-kodelister/havnedata/fenderorientering</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-fendertype"></a>«CodeList» Fendertype

**Definisjon:** Angivelse av ulike fendertyper.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/fendertype">https://register.geonorge.no/sosi-kodelister/havnedata/fendertype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-avfallstype"></a>«CodeList» Avfallstype

**Definisjon:** Angir type avfall.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/avfallstype">https://register.geonorge.no/sosi-kodelister/havnedata/avfallstype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-beholdertype"></a>«CodeList» Beholdertype

**Definisjon:** Angir type avfallsbeholder.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/beholdertype">https://register.geonorge.no/sosi-kodelister/havnedata/beholdertype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-kaidekketype"></a>«CodeList» Kaidekketype

**Definisjon:** Angivelse av ulike typer dekke på kai.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/kaidekketype">https://register.geonorge.no/sosi-kodelister/havnedata/kaidekketype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-kaitype"></a>«CodeList» Kaitype

**Definisjon:** Angivelse av ulik bruk av kai.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/kaitype">https://register.geonorge.no/sosi-kodelister/havnedata/kaitype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-fortøyningstype"></a>«CodeList» Fortøyningstype

**Definisjon:** Type fortøyningsinnretning.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/fortoyningstype">https://register.geonorge.no/sosi-kodelister/havnedata/fortoyningstype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-måned"></a>«CodeList» Måned

**Definisjon:** Kodeliste over årets måneder.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/maned">https://register.geonorge.no/sosi-kodelister/havnedata/maned</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-avsperringstype"></a>«CodeList» Avsperringstype

**Definisjon:** Type avsperring for HavnegjerdeInngang.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/avsperringstype">https://register.geonorge.no/sosi-kodelister/havnedata/avsperringstype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-åpningstype"></a>«CodeList» Åpningstype

**Definisjon:** Beskriver åpningsmekanisme av port, bom eller annen avsperringstype for HavnegjerdeInngang.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/apningstype">https://register.geonorge.no/sosi-kodelister/havnedata/apningstype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-beredskapstype"></a>«CodeList» Beredskapstype

**Definisjon:** Angir type beredskap eller beredskapsutstyr.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/beredskapstype">https://register.geonorge.no/sosi-kodelister/havnedata/beredskapstype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-kaifronttype"></a>«CodeList» Kaifronttype

**Definisjon:** Ulike typer kaifronter. Beskriver kaifronten sin konstruksjon mot sjøen.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/kaifronttype">https://register.geonorge.no/sosi-kodelister/havnedata/kaifronttype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-sensortype"></a>«CodeList» Sensortype

**Definisjon:** Type sensor.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/sensortype">https://register.geonorge.no/sosi-kodelister/havnedata/sensortype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-bruksklassetype"></a>«CodeList» Bruksklassetype

**Definisjon:** Kodelisten angir bruksklasse på kai. Bruksklassetype er kodeliste for egenskap bruksklasse på objekttype Lastbegrensningsområde. Bruksklassen forkortes Bk og etterfølges av et tall. Den angir største tillatte aksellast, last fra akselkombinasjoner og totalvekt avhengig av avstanden mellom akslene. Som beskrevet i "Forskrift om bruk av kjøretøy" og Statens vegvesen sin håndbok R412.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/bruksklassetype">https://register.geonorge.no/sosi-kodelister/havnedata/bruksklassetype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-drivstofftype"></a>«CodeList» Drivstofftype

**Definisjon:** Angir hvilke typer drivstoff som kan fylles.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/drivstofftype">https://register.geonorge.no/sosi-kodelister/havnedata/drivstofftype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-avløpstype"></a>«CodeList» Avløpstype

**Definisjon:** Angir hvilken type væske som kan tømmes.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/avlopstype">https://register.geonorge.no/sosi-kodelister/havnedata/avlopstype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-elanleggstype"></a>«CodeList» ELanleggstype

**Definisjon:** Type EL-anlegg/strømanlegg.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/elanleggstype">https://register.geonorge.no/sosi-kodelister/havnedata/elanleggstype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-frekvens"></a>«CodeList» Frekvens

**Definisjon:** Angir frekvensen for EL-koblingen, som er hvor mange ganger en elektrisk spenning veksler i løpet av ett sekund. Måles i Hz.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/frekvens">https://register.geonorge.no/sosi-kodelister/havnedata/frekvens</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-spenning"></a>«CodeList» Spenning

**Definisjon:** Kodeliste for å angi den eletriske spenningen. Måleenhet i volt.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/spenning">https://register.geonorge.no/sosi-kodelister/havnedata/spenning</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-datafangstmetode"></a>«CodeList» Datafangstmetode

**Definisjon:** Metode for datafangst. Datafangstmetoden beskriver hvordan selve vektordataene er posisjonert fra et datagrunnlag (observasjoner med landmålingsutstyr, fotogrammetrisk stereomodell, digital terrengmodell etc.) og ikke prosessen med å innhente det bakenforliggende datagrunnlaget.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/datafangstmetode">https://register.geonorge.no/sosi-kodelister/havnedata/datafangstmetode</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-synbarhet"></a>«CodeList» Synbarhet

**Definisjon:** hvor godt den kartlagte detalj var synbar ved kartleggingen

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/synbarhet">https://register.geonorge.no/sosi-kodelister/havnedata/synbarhet</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-forbudstype"></a>«CodeList» Forbudstype

**Definisjon:** Kodeliste for å angi forbudstype for forbudsområde.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/forbudstype">https://register.geonorge.no/sosi-kodelister/havnedata/forbudstype</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-fartøytype"></a>«CodeList» Fartøytype

**Definisjon:** Kodeliste for å spesifisere hvilket type fartøy en regulering eller restriksjon omfatter.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/havnedata/fartoytype">https://register.geonorge.no/sosi-kodelister/havnedata/fartoytype</a></td>
    </tr>
  </tbody>
</table>
