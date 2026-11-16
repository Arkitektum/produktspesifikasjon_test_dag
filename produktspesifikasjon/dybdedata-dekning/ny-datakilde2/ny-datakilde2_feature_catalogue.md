#### Feature

Kun plassholder for original klasse. Fjernes fra XSD.

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
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
AnyFeature

**Assosiasjoner**
PropertySet – rolle: propertySet – kardinalitet: 0..*
PropertySet – rolle: propertySet – kardinalitet: 0..*
Property – rolle: property – kardinalitet: 0..*
Property – rolle: property – kardinalitet: 0..*

#### LandSurface

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
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>TIN</td>
      <td>1</td>
    </tr>
    <tr>
      <td>material</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

#### PhysicalElement

Kun plassholder for original klasse. Fjernes fra XSD.

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
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Feature

**Assosiasjoner**
PhysicalElement – rolle: part – kardinalitet: 0..*
PhysicalElement – rolle: partOf – kardinalitet: 0..1

#### Facility

Facilities include buildings and civil engineering works and their associated siteworks.  Civil engineering works, or infrastructure facilities, are construction works comprising a structure, such as a dam, bridge, road, railway, runway, utilities, pipeline, or sewerage system, or are the result of operations such as dredging, earthwork, and geotechnical processes.<br />A facility has a life cycle, including planning, design, construction, maintenance, operation, and removal phases  The design and construction phases are typically performed as part of a project.  There may be multiple such projects during the life cycle of the facility to enable phased construction and incremental improvement.

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
      <td>facility<wbr />ID</td>
      <td></td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>type</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td></td>
      <td>Status</td>
      <td>1</td>
    </tr>
    <tr>
      <td>footprint</td>
      <td></td>
      <td>geometry-any</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Feature

#### FacilityPart

Land and Infrastructure facility, such as a road or bridge.  A facility has a life cycle, including planning, design, construction, maintenance, operation, and removal phases  The design and construction phases are typically performed as part of a project.  There may be multiple such projects during the life cycle of the facility to enable phased construction and incremental improvement.

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
      <td>facility<wbr />Part<wbr />ID</td>
      <td></td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>type</td>
      <td></td>
      <td><a href="#kodeliste-facilityparttype">Facility<wbr />Part<wbr />Type</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td></td>
      <td>Status</td>
      <td>1</td>
    </tr>
    <tr>
      <td>footprint</td>
      <td></td>
      <td>geometry-any</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>alternative</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Feature

**Assosiasjoner**
Facility
FacilityPartRelationship – rolle: relationship – kardinalitet: 0..*

#### Alignment

PositioningElement which provides a Linear Referencing System for locating PhysicalElements.<br />An Alignment shall be continuous, non-branching, and non-overlapping. If it is a Project Alignment, it is for a single alternative, as specified by its owning ProjectPart.<br /><br />Kun plassholder for original klasse. Fjernes fra XSD.

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
      <td>alignment<wbr />ID</td>
      <td></td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>design<wbr />Alternative</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>purpose</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>linestring2<wbr />DRepresentation</td>
      <td></td>
      <td>Line<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>linestring3<wbr />DRepresentation</td>
      <td></td>
      <td>Line<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Feature

#### Road

that part of a Project that relates to a single alternative for a single Road part of a project for a single Road part of a Facility.  Each alternative is a separate Road ProjectPart.  An alternative may be a design alternative or a separate phase of construction.<br /><br />Kun plassholder for original klasse. Fjernes fra XSD.

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
      <td>approximate<wbr />Width</td>
      <td></td>
      <td>Length</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FacilityPart</th>
    </tr>
    <tr>
      <td>facility<wbr />Part<wbr />ID</td>
      <td></td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>type</td>
      <td></td>
      <td><a href="#kodeliste-facilityparttype">Facility<wbr />Part<wbr />Type</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td></td>
      <td>Status</td>
      <td>1</td>
    </tr>
    <tr>
      <td>footprint</td>
      <td></td>
      <td>geometry-any</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>alternative</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
FacilityPart

**Assosiasjoner**
Alignment – rolle: alignment – kardinalitet: 0..*
RoadElementSet – rolle: roadElementSet – kardinalitet: 0..*
StringLine – rolle: stringLine – kardinalitet: 0..*
StringLineSet – rolle: stringLineSet – kardinalitet: 0..*
CrossSection – rolle: crossSection – kardinalitet: 0..*
RoadElement – rolle: element – kardinalitet: 0..*

#### RoadElement

Kun plassholder for original klasse. Fjernes fra XSD.

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
      <td>road<wbr />Element<wbr />ID</td>
      <td></td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>road<wbr />Element<wbr />Type</td>
      <td></td>
      <td><a href="#kodeliste-roadelementtype">Road<wbr />Element<wbr />Type</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>material</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
PhysicalElement

**Assosiasjoner**
LinearElement – rolle: locatedAlong – kardinalitet: 0..1
RoadElementSet

#### AnyFeature

Også kalla AbstractFeature i LandInfra

Egenskaper

(ingen)

#### AbstractFeature

Kun plassholder for original klasse. Fjernes fra XSD.

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
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Feature

**Assosiasjoner**
AbstractFeature – rolle: part – kardinalitet: 0..*
AbstractFeature – rolle: partOf – kardinalitet: 0..1

#### Alignment

PositioningElement which provides a Linear Referencing System for locating PhysicalElements.<br />An Alignment shall be continuous, non-branching, and non-overlapping. If it is a Project Alignment, it is for a single alternative, as specified by its owning ProjectPart.

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
      <td>alignment<wbr />ID</td>
      <td></td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>purpose</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>design<wbr />Altenrative</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>linestring2<wbr />DRepresentation</td>
      <td></td>
      <td>Line<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>linestring3<wbr />DRepresentation</td>
      <td></td>
      <td>Line<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Assosiasjoner**
AlignmentCurve – rolle: geometry – kardinalitet: 0..1

#### Referanselinje

Referanselinje er en linje som brukes som referanse for flater. Kan være senterlinje eller andre flate avgrensninger.

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
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte linja til "norsk vegbygging".<br />Norske tillegg er begreper tilpasset norsk vegbygging.</td>
      <td>Referanse<wbr />Linje<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Alignment</th>
    </tr>
    <tr>
      <td>alignment<wbr />ID</td>
      <td></td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>design<wbr />Alternative</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>purpose</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>linestring2<wbr />DRepresentation</td>
      <td></td>
      <td>Line<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>linestring3<wbr />DRepresentation</td>
      <td></td>
      <td>Line<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Alignment

#### VegElement (abstrakt)

fornorsking av RoadElement, for å kunne knytte til norsk vegbyggings-terminologi.

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
      <td>fra<wbr />Profil</td>
      <td>startprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>til<wbr />Profil</td>
      <td>sluttprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegelementet til norsk vegbygging-terminologi.</td>
      <td>Veg<wbr />Element<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponentreferanse</td>
      <td>referanse til ekstern database, der mer om objektet finnes.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra RoadElementN</th>
    </tr>
    <tr>
      <td>road<wbr />Element<wbr />ID</td>
      <td>ID for vegelementet</td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>material</td>
      <td>angivelse av material for vegelementet, fritekst.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
RoadElementN

#### Veg

fornorsking av landInfra/Road, for å kunne knytte til norske tillegg.

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
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegen til "norsk vegbygging-teori".</td>
      <td>Veg<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponent<wbr />Referanse</td>
      <td>Henviser til mer informasjon om en komponent gitt i kodeliste Komponentreferanse.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- dimensjonerende<wbr />Parametre</td>
      <td>samlingen av dimensjonerende verdier for vegen gitt i kodeliste DimensjonerendeParametere_Veg.</td>
      <td>Dimensjonerende<wbr />Verdier_<wbr />Veg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - standardklasse<wbr />Vegstandard</td>
      <td>Standard vegklasse</td>
      <td><a href="#kodeliste-dimensjoneringsklasse">Dimensjoneringsklasse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - hastighet</td>
      <td>Dimensjonerende hastighet for vegen</td>
      <td><a href="#kodeliste-dimensjonerendehastighet">Dimensjonerende<wbr />Hastighet</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - vegbredde</td>
      <td>Dimensjonerende vegbredde for vegen</td>
      <td><a href="#kodeliste-dimensjonerendevegbredde">Dimensjonerende<wbr />Vegbredde</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - motorkjøretøy</td>
      <td>Dimensjonerende motorkjøretøytype for vegen</td>
      <td><a href="#kodeliste-dimensjonerendemotorkjøretøy">Dimensjonerende<wbr />Motorkjøretøy</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - trafikkmengde<wbr />ÅDT</td>
      <td>Dimensjonerende trafikkmengde målt i ÅDT for vegen</td>
      <td><a href="#kodeliste-dimensjonerendetrafikkmengdeådt">Dimensjonerende<wbr />Trafikkmengde<wbr />ÅDT</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kjøremåte</td>
      <td>Dimensjonerende kjøremåte for vegen</td>
      <td><a href="#kodeliste-dimensjonerendekjøremåte">Dimensjonerende<wbr />Kjøremåte</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - max<wbr />Overhøyde<wbr />Prosent</td>
      <td>Max tverrfall i prosent</td>
      <td><a href="#kodeliste-maxoverhøydeprosent">Max<wbr />Overhøyde<wbr />Prosent</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - trafikk</td>
      <td>Dimensjonerende trafikk målt i aksel-last for vegen</td>
      <td><a href="#kodeliste-dimensjonerendetrafikkgruppe">Dimensjonerende<wbr />Trafikkgruppe</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- total<wbr />Overbygningstykkelse</td>
      <td>totaltykkelsen på overbygningen, angitt i meter</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Road</th>
    </tr>
    <tr>
      <td>approximate<wbr />Width</td>
      <td></td>
      <td>Length</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra FacilityPart</th>
    </tr>
    <tr>
      <td>facility<wbr />Part<wbr />ID</td>
      <td></td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>type</td>
      <td></td>
      <td><a href="#kodeliste-facilityparttype">Facility<wbr />Part<wbr />Type</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>status</td>
      <td></td>
      <td>Status</td>
      <td>1</td>
    </tr>
    <tr>
      <td>footprint</td>
      <td></td>
      <td>geometry-any</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>alternative</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Road

**Assosiasjoner**
Referanselinje – rolle: referanselinje – kardinalitet: 0..*
VegElement – rolle: element – kardinalitet: 0..*

#### RoadElementN (abstrakt)

Hensikt: Ta bort kodeliste RoadElementType fra RoadElement

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
      <td>road<wbr />Element<wbr />ID</td>
      <td>ID for vegelementet</td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>material</td>
      <td>angivelse av material for vegelementet, fritekst.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
PhysicalElement

#### Overbygningselement_for_Vegdesign

Overbygningselement_for_Vegdesign skal ha betegnelse i henhold til kodeliste OverbygningLagtype, og i henhold til lag i overbygningen beskrevet i N200.<br />Link til N200 + eventuelt figur.

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
      <td>name</td>
      <td>navn på elementet, fritekst</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lagtype</td>
      <td>lagtypen på laget, gitt ved kodelisteverdi</td>
      <td><a href="#kodeliste-overbygninglagtype">Overbygning<wbr />Lagtype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lagnummer</td>
      <td>nummer på laget, nummerert fra toppen og nedover</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tykkelse</td>
      <td>tykkelsen på laget, gitt i meter</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>indre<wbr />Fyllingshelling</td>
      <td>brukes til å angi at laget ikke kun ligger under vegdesignelementet, men at fylingen skrår utover. Angis som desimaltall</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

#### VegdesignElement

VegdesignElement er flateelementer topp vegkonstruksjon inkludert både kjøreflater og alle andre overflater til og med fylling/skjæring. Flatebetegnelsene framkommer i union av flere kodelister. Unionen av kodelister er VegdesignElementType. Noen flater har regelverk knyttet til seg, for eksempel kjøreflater.<br />Andre benyttes for å sette av plass til for eksempel rekkverk, busslomme, overvannshåndtering eller landskapsforming.

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
      <td>veg<wbr />Design</td>
      <td>flatetypen dette vegdesignelementet tilhører</td>
      <td>Vegdesign<wbr />Ref<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- flatetype</td>
      <td>angivelse av hva slags vegdesignflatetype dette gjelder</td>
      <td>Vegdesign<wbr />Element<wbr />Type</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- flaterekkefølge</td>
      <td>rekkefølge på flaten stringlinen representerer i vegdesignet</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- vegside</td>
      <td>angivelse av vegside, etter kodeliste. NB! Erstatter tidligere praksisk med positivt og negativt tall.</td>
      <td><a href="#kodeliste-side">Side</a><br />(enumerering)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>ytterkant</td>
      <td>ytterkant på elementet</td>
      <td>Ytterkant</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra VegElement</th>
    </tr>
    <tr>
      <td>fra<wbr />Profil</td>
      <td>startprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>til<wbr />Profil</td>
      <td>sluttprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegelementet til norsk vegbygging-terminologi.</td>
      <td>Veg<wbr />Element<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponentreferanse</td>
      <td>referanse til ekstern database, der mer om objektet finnes.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra RoadElementN</th>
    </tr>
    <tr>
      <td>road<wbr />Element<wbr />ID</td>
      <td>ID for vegelementet</td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>material</td>
      <td>angivelse av material for vegelementet, fritekst.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
VegElement

**Assosiasjoner**
Overbygningselement_for_Vegdesign – rolle: overbygning – kardinalitet: 0..*
Underbygning – rolle: underbygning – kardinalitet: 0..*
Planum – rolle: planum – kardinalitet: 0..*

#### Planum

Planum kalles også traubunn, og er overflaten av underbygningen.<br />Traubunn er graveflate som graves ut, eller toppflate bearbeidet undergrunn som gjøres før oppbygging av overbygning. ved bygging av veg,

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
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra VegElement</th>
    </tr>
    <tr>
      <td>fra<wbr />Profil</td>
      <td>startprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>til<wbr />Profil</td>
      <td>sluttprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegelementet til norsk vegbygging-terminologi.</td>
      <td>Veg<wbr />Element<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponentreferanse</td>
      <td>referanse til ekstern database, der mer om objektet finnes.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra RoadElementN</th>
    </tr>
    <tr>
      <td>road<wbr />Element<wbr />ID</td>
      <td>ID for vegelementet</td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>material</td>
      <td>angivelse av material for vegelementet, fritekst.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
VegkroppElement

**Assosiasjoner**
YtreFlatekant – rolle: venstreSide – kardinalitet: 0..1
YtreFlatekant – rolle: høyreSide – kardinalitet: 0..1

#### Overbygning

Den del av vegkroppen som er over traubunn/planum.<br />Overbygningen kan bestå av frostsikringslag, filterlag (ev. fiberduk), forsterkningslag, bærelag og dekke (bindlag/bindelag og slitelag).

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
      <td>lagtype</td>
      <td>Betegnelse på fysisk lag i overbygningen  i henhold til kodeliste OverbygningLagtype.</td>
      <td><a href="#kodeliste-overbygninglagtype">Overbygning<wbr />Lagtype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lagnummer</td>
      <td>Lagene nummereres fra toppen, dvs ofte  VegdekkeSlitelag som nr 1</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tykkelse</td>
      <td>tykkelse på laget, enhet meter</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra VegElement</th>
    </tr>
    <tr>
      <td>fra<wbr />Profil</td>
      <td>startprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>til<wbr />Profil</td>
      <td>sluttprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegelementet til norsk vegbygging-terminologi.</td>
      <td>Veg<wbr />Element<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponentreferanse</td>
      <td>referanse til ekstern database, der mer om objektet finnes.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra RoadElementN</th>
    </tr>
    <tr>
      <td>road<wbr />Element<wbr />ID</td>
      <td>ID for vegelementet</td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>material</td>
      <td>angivelse av material for vegelementet, fritekst.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
VegkroppElement

**Assosiasjoner**
VegdesignElement – rolle: vegdesignElement – kardinalitet: 0..1

#### VegkroppElement (abstrakt)

Fysisk del av Overbygning, Underbygning. eller Planum.

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
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra VegElement</th>
    </tr>
    <tr>
      <td>fra<wbr />Profil</td>
      <td>startprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>til<wbr />Profil</td>
      <td>sluttprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegelementet til norsk vegbygging-terminologi.</td>
      <td>Veg<wbr />Element<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponentreferanse</td>
      <td>referanse til ekstern database, der mer om objektet finnes.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra RoadElementN</th>
    </tr>
    <tr>
      <td>road<wbr />Element<wbr />ID</td>
      <td>ID for vegelementet</td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>material</td>
      <td>angivelse av material for vegelementet, fritekst.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
VegElement

**Assosiasjoner**
Volumobjekt – rolle: volum – kardinalitet: 0..1
ToppOverflate – rolle: toppOverflate – kardinalitet: 0..1
YtreFlatekant – rolle: ytterkant – kardinalitet: 0..1

#### Underbygning

Den del av vegkroppen som er under traubunn/planum.<br />Underbygningen kan bestå av fylling, undergrunn og undergrunn, forbedret.

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
      <td>lagtype</td>
      <td>Betegnelse på fysisk lag i underbygningen  i henhold til kodeliste UnderbygningLagtype.</td>
      <td><a href="#kodeliste-underbygninglagtype">Underbygning<wbr />Lagtype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lagnummer</td>
      <td>lagnummer, nummerert i stigende rekkefølge fra planum = 0  og nedover.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tykkelse</td>
      <td>tykkelse på laget, enhet meter.</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra VegElement</th>
    </tr>
    <tr>
      <td>fra<wbr />Profil</td>
      <td>startprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>til<wbr />Profil</td>
      <td>sluttprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegelementet til norsk vegbygging-terminologi.</td>
      <td>Veg<wbr />Element<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponentreferanse</td>
      <td>referanse til ekstern database, der mer om objektet finnes.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra RoadElementN</th>
    </tr>
    <tr>
      <td>road<wbr />Element<wbr />ID</td>
      <td>ID for vegelementet</td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>material</td>
      <td>angivelse av material for vegelementet, fritekst.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
VegkroppElement

#### Sideområde

Den delen av vegoverflata som ligger på sida av vegkroppen og som ikke er knytta til noen overbygning

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
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra VegElement</th>
    </tr>
    <tr>
      <td>fra<wbr />Profil</td>
      <td>startprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>til<wbr />Profil</td>
      <td>sluttprofil for dette vegelementet</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegelementet til norsk vegbygging-terminologi.</td>
      <td>Veg<wbr />Element<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponentreferanse</td>
      <td>referanse til ekstern database, der mer om objektet finnes.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra RoadElementN</th>
    </tr>
    <tr>
      <td>road<wbr />Element<wbr />ID</td>
      <td>ID for vegelementet</td>
      <td>ID</td>
      <td>1</td>
    </tr>
    <tr>
      <td>material</td>
      <td>angivelse av material for vegelementet, fritekst.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Feature</th>
    </tr>
    <tr>
      <td>name</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>description</td>
      <td></td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>spatial<wbr />Representation</td>
      <td></td>
      <td>Spatial<wbr />Representation</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>linearly<wbr />Referenced<wbr />Location</td>
      <td></td>
      <td>Linearly<wbr />Referenced<wbr />Location</td>
      <td>0..*</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
VegkroppElement

**Assosiasjoner**
VegdesignElement – rolle: vegdesignElement – kardinalitet: 0..1

#### GenerelleEgenskaper

Abstrakt supertype med generelle egenskaper fra SOSI Del 1 og LandInfra

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
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

#### Vegkropp

Vegens overbygning og underbygning, samt planum.

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
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
GenerelleEgenskaper

**Assosiasjoner**
VegKroppElement – rolle: vegkroppElement – kardinalitet: 0..*

#### Veg_Prosjektreferanse

fornorsking av landInfra/Road, for å kunne knytte til norske tillegg.

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
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegen til "norsk vegbygging-teori".</td>
      <td>Veg<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponent<wbr />Referanse</td>
      <td>Henviser til mer informasjon om en komponent gitt i kodeliste Komponentreferanse.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- dimensjonerende<wbr />Parametre</td>
      <td>samlingen av dimensjonerende verdier for vegen gitt i kodeliste DimensjonerendeParametere_Veg.</td>
      <td>Dimensjonerende<wbr />Verdier_<wbr />Veg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - standardklasse<wbr />Vegstandard</td>
      <td>Standard vegklasse</td>
      <td><a href="#kodeliste-dimensjoneringsklasse">Dimensjoneringsklasse</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - hastighet</td>
      <td>Dimensjonerende hastighet for vegen</td>
      <td><a href="#kodeliste-dimensjonerendehastighet">Dimensjonerende<wbr />Hastighet</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - vegbredde</td>
      <td>Dimensjonerende vegbredde for vegen</td>
      <td><a href="#kodeliste-dimensjonerendevegbredde">Dimensjonerende<wbr />Vegbredde</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - motorkjøretøy</td>
      <td>Dimensjonerende motorkjøretøytype for vegen</td>
      <td><a href="#kodeliste-dimensjonerendemotorkjøretøy">Dimensjonerende<wbr />Motorkjøretøy</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - trafikkmengde<wbr />ÅDT</td>
      <td>Dimensjonerende trafikkmengde målt i ÅDT for vegen</td>
      <td><a href="#kodeliste-dimensjonerendetrafikkmengdeådt">Dimensjonerende<wbr />Trafikkmengde<wbr />ÅDT</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kjøremåte</td>
      <td>Dimensjonerende kjøremåte for vegen</td>
      <td><a href="#kodeliste-dimensjonerendekjøremåte">Dimensjonerende<wbr />Kjøremåte</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - max<wbr />Overhøyde<wbr />Prosent</td>
      <td>Max tverrfall i prosent</td>
      <td><a href="#kodeliste-maxoverhøydeprosent">Max<wbr />Overhøyde<wbr />Prosent</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - trafikk</td>
      <td>Dimensjonerende trafikk målt i aksel-last for vegen</td>
      <td><a href="#kodeliste-dimensjonerendetrafikkgruppe">Dimensjonerende<wbr />Trafikkgruppe</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- total<wbr />Overbygningstykkelse</td>
      <td>totaltykkelsen på overbygningen, angitt i meter</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
GenerelleEgenskaper

**Assosiasjoner**
Vegkropp – rolle: vegelementsamling – kardinalitet: 0..*
VegKroppElement – rolle: element – kardinalitet: 0..*
StringLineN – rolle: stringLine – kardinalitet: 0..*

#### StringLineN_Planum

Linje som beskriver planum/traubunn.<br />Oftest beregnet med ett punkt pr generert tverrprofil, og lenket sammen.

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
      <td>vegdesign<wbr />Ref</td>
      <td>referanse til vegdesinget som linja er avledet fra</td>
      <td>Vegdesign<wbr />Ref<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- flatetype</td>
      <td>angivelse av hva slags vegdesignflatetype dette gjelder</td>
      <td>Vegdesign<wbr />Element<wbr />Type</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- flaterekkefølge</td>
      <td>rekkefølge på flaten stringlinen representerer i vegdesignet</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- vegside</td>
      <td>angivelse av vegside, etter kodeliste. NB! Erstatter tidligere praksisk med positivt og negativt tall.</td>
      <td><a href="#kodeliste-side">Side</a><br />(enumerering)</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra StringLineN</th>
    </tr>
    <tr>
      <td>geometri</td>
      <td>linjas geometri</td>
      <td>GM_<wbr />Curve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
StringLineN

#### StringLineN_Referanselinje

Spesifikk linje som vegelement(er) refererer seg til

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
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra StringLineN</th>
    </tr>
    <tr>
      <td>geometri</td>
      <td>linjas geometri</td>
      <td>GM_<wbr />Curve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
StringLineN

#### StringLineN_Underbygning

Linjer som beskriver lag/flate i underbygning.<br />Oftest beregnet med ett punkt pr generert tverrprofil, og lenket sammen.

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
      <td>lagtype</td>
      <td>navn på underbygninglaget som linja representerer</td>
      <td><a href="#kodeliste-underbygninglagtype">Underbygning<wbr />Lagtype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>vegdesign<wbr />Ref</td>
      <td>referanse til vegdesinget som linja er avledet fra</td>
      <td>Vegdesign<wbr />Ref<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- flatetype</td>
      <td>angivelse av hva slags vegdesignflatetype dette gjelder</td>
      <td>Vegdesign<wbr />Element<wbr />Type</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- flaterekkefølge</td>
      <td>rekkefølge på flaten stringlinen representerer i vegdesignet</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- vegside</td>
      <td>angivelse av vegside, etter kodeliste. NB! Erstatter tidligere praksisk med positivt og negativt tall.</td>
      <td><a href="#kodeliste-side">Side</a><br />(enumerering)</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra StringLineN</th>
    </tr>
    <tr>
      <td>geometri</td>
      <td>linjas geometri</td>
      <td>GM_<wbr />Curve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
StringLineN

#### StringLineN

linjer som går langs  vegen.<br />Oftest beregnet med ett punkt pr generert tverrprofil, og lenket sammen.

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
      <td>geometri</td>
      <td>linjas geometri</td>
      <td>GM_<wbr />Curve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
GenerelleEgenskaper

#### StringLineN_Sideområde

Linjer som beskriver sideområde av veg.<br />Oftest beregnet med ett punkt pr generert tverrprofil, og lenket sammen.

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
      <td>vegdesign<wbr />Ref</td>
      <td>referanse til vegdesinget som linja er avledet fra</td>
      <td>Vegdesign<wbr />Ref<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- flatetype</td>
      <td>angivelse av hva slags vegdesignflatetype dette gjelder</td>
      <td>Vegdesign<wbr />Element<wbr />Type</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- flaterekkefølge</td>
      <td>rekkefølge på flaten stringlinen representerer i vegdesignet</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- vegside</td>
      <td>angivelse av vegside, etter kodeliste. NB! Erstatter tidligere praksisk med positivt og negativt tall.</td>
      <td><a href="#kodeliste-side">Side</a><br />(enumerering)</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra StringLineN</th>
    </tr>
    <tr>
      <td>geometri</td>
      <td>linjas geometri</td>
      <td>GM_<wbr />Curve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
StringLineN

#### StringLineN_Overbygning

Linjer som beskriver overbygningslag.<br />Oftest beregnet med ett punkt pr generert tverrprofil, og lenket sammen.

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
      <td>lagtype</td>
      <td>navn på overbygninglaget som linja representerer</td>
      <td><a href="#kodeliste-overbygninglagtype">Overbygning<wbr />Lagtype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>vegdesign<wbr />Ref</td>
      <td>referanse til vegdesinget som linja er avledet fra</td>
      <td>Vegdesign<wbr />Ref<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- flatetype</td>
      <td>angivelse av hva slags vegdesignflatetype dette gjelder</td>
      <td>Vegdesign<wbr />Element<wbr />Type</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- flaterekkefølge</td>
      <td>rekkefølge på flaten stringlinen representerer i vegdesignet</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- vegside</td>
      <td>angivelse av vegside, etter kodeliste. NB! Erstatter tidligere praksisk med positivt og negativt tall.</td>
      <td><a href="#kodeliste-side">Side</a><br />(enumerering)</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra StringLineN</th>
    </tr>
    <tr>
      <td>geometri</td>
      <td>linjas geometri</td>
      <td>GM_<wbr />Curve</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
StringLineN

#### VegdesignElement_for_Vegkropp

VegdesignElement er flateelementer topp vegkonstruksjon inkludert både kjøreflater og alle andre overflater til og med fylling/skjæring. Flatebetegnelsene framkommer i union av flere kodelister. Unionen av kodelister er VegdesignElementType. Noen flater har regelverk knyttet til seg, for eksempel kjøreflater.<br />Andre benyttes for å sette av plass til for eksempel rekkverk, busslomme, overvannshåndtering eller landskapsforming.

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
      <td>veg<wbr />Design</td>
      <td>flatetypen dette vegdesignelementet tilhører</td>
      <td>Vegdesign<wbr />Ref<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- flatetype</td>
      <td>angivelse av hva slags vegdesignflatetype dette gjelder</td>
      <td>Vegdesign<wbr />Element<wbr />Type</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- flaterekkefølge</td>
      <td>rekkefølge på flaten stringlinen representerer i vegdesignet</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- vegside</td>
      <td>angivelse av vegside, etter kodeliste. NB! Erstatter tidligere praksisk med positivt og negativt tall.</td>
      <td><a href="#kodeliste-side">Side</a><br />(enumerering)</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
GenerelleEgenskaper

#### Planum

Planum kalles også traubunn, og er overflaten av underebygningen.<br />Traubunn er graveflate som graves ut, eller toppflate bearbeidet undergrunn som gjøres før oppbygging av overbygning. ved bygging av veg,

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
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra VegKroppElement</th>
    </tr>
    <tr>
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegelementet til "norsk vegbygging-teori".</td>
      <td>Veg<wbr />Element<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponentreferanse</td>
      <td>referanse til ekstern database, der mer om objektet finnes.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
VegKroppElement

**Assosiasjoner**
YtreFlatekant – rolle: høyreSide – kardinalitet: 0..1
YtreFlatekant – rolle: venstreSide – kardinalitet: 0..1

#### VegKroppElement (abstrakt)

fornorsking av RoadElement, for å kunne knytte til norsk vegbyggings-teori

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
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegelementet til "norsk vegbygging-teori".</td>
      <td>Veg<wbr />Element<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponentreferanse</td>
      <td>referanse til ekstern database, der mer om objektet finnes.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
GenerelleEgenskaper

**Assosiasjoner**
ToppOverflate – rolle: toppOverflate – kardinalitet: 0..1
YtreFlatekant – rolle: ytterkant – kardinalitet: 0..1
Volumobjekt – rolle: volum – kardinalitet: 0..1

#### Underbygning

En fellesbetegnelse for undergrunn, forbedret og fylling opp til planum.<br />Den del av vegkroppen som er under traubunn/planum.<br />Underbygningen kan bestå av fylling, undergrunn og undergrunn, forbedret.

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
      <td>lagtype</td>
      <td>Betegnelse på fysisk lag i underbygningen  i henhold til kodeliste UnderbygningLagtype.</td>
      <td><a href="#kodeliste-underbygninglagtype">Underbygning<wbr />Lagtype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lagnummer</td>
      <td>lagnummer, nummerert i stigende rekkefølge fra planum = 0  og nedover.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tykkelse</td>
      <td>tykkelse på laget, enhet meter</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra VegKroppElement</th>
    </tr>
    <tr>
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegelementet til "norsk vegbygging-teori".</td>
      <td>Veg<wbr />Element<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponentreferanse</td>
      <td>referanse til ekstern database, der mer om objektet finnes.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
VegKroppElement

#### Overbygning

Den del av vegkroppen som er over traubunn/planum.<br />Overbygningen kan bestå av frostsikringslag, filterlag (ev. fiberduk), forsterkningslag, bærelag og dekke (bindlag/bindelag og slitelag).

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
      <td>lagtype</td>
      <td>Betegnelse på fysisk lag i overbygningen  i henhold til kodeliste OverbygningLagtype.</td>
      <td><a href="#kodeliste-overbygninglagtype">Overbygning<wbr />Lagtype</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>lagnummer</td>
      <td>Lagene nummereres fra toppen, dvs ofte  VegdekkeSlitelag som nr 1</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tykkelse</td>
      <td>tykkelse på laget, enhet meter</td>
      <td>Real</td>
      <td>0..1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra VegKroppElement</th>
    </tr>
    <tr>
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegelementet til "norsk vegbygging-teori".</td>
      <td>Veg<wbr />Element<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponentreferanse</td>
      <td>referanse til ekstern database, der mer om objektet finnes.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
VegKroppElement

**Assosiasjoner**
VegdesignElement_for_Vegkropp – rolle: vegdesignElement – kardinalitet: 0..1

#### Sideområde

Den delen av vegoverflata som ligger på sida av vegkroppen og som ikke er knytta til noen overbygning

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
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra VegKroppElement</th>
    </tr>
    <tr>
      <td>norske<wbr />Tillegg</td>
      <td>angivelse av tilleggsverdier for å knytte vegelementet til "norsk vegbygging-teori".</td>
      <td>Veg<wbr />Element<wbr />Norske<wbr />Tillegg<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- tilhører<wbr />Prosjekt</td>
      <td>identifikasjon av prosjektet leveransen tilhører</td>
      <td>Prosjektreferanse<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - oppdragsgiver<wbr />Navn</td>
      <td>navn på oppdragsgiver</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - oppdragsgivers<wbr />Organisasjonsnummer</td>
      <td>oppdragsgivers organisasjonsnummer</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - prosjektnavn</td>
      <td>Oppdragsgivers prosjektnavn</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />ID</td>
      <td>Oppdragsgivers prosjektID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjektfase</td>
      <td>Prosjektfase i henhold til faser definert for prosjektet</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - fasestatus</td>
      <td>Status på dataleveransen i forhold til fasen.<br />Fasebetegnelsen som brukes må finnes i oppdragsgivers liste over definerte faser for prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - levert<wbr />Av<wbr />Organisasjon</td>
      <td>navn på organisasjon/firma som er ansvarlig for leveransen</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - utarbeidet<wbr />Av</td>
      <td>Navn på kontaktperson hos den som har utarbeidet datasettet</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - prosjekt<wbr />URL</td>
      <td>URL til prosjektdatabasen det mer informasjon om prosjektet kan finnes.<br />Merknad: Det antas at prosjektdatabasen også kan inneholde informasjon om andre prosjekt, og at noen av de andre egenskapene på dette objektet må brukes for å søke fram det rette prosjektet og del/fase av prosjektet.</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- - leveransedato</td>
      <td>Dato for leveransen. Bør entydig identifisere leveranse, dvs to leveranser til samme prosjekt/fase/status kan ikke ha samme leveransedato</td>
      <td>Date</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- komponentreferanse</td>
      <td>referanse til ekstern database, der mer om objektet finnes.</td>
      <td>Komponentreferanse<br />(datatype)</td>
      <td>0..*</td>
    </tr>
    <tr>
      <td>- - komponentkodesystem</td>
      <td>Navnet på kodesystemet som brukes (velges fra kodeliste).</td>
      <td><a href="#kodeliste-komponentkodesystem">Komponentkodesystem</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - kodesystemversjon</td>
      <td>versjonen på komponentkodesystemet (dersom slikt finnes)</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- - komponentkodeverdi</td>
      <td>Identifikasjonen på komponenten i oppgitt kodesystem</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
VegKroppElement

**Assosiasjoner**
VegdesignElement_for_Vegkropp – rolle: vegdesignElement – kardinalitet: 0..1

#### Terrengflate

Tatt med LandSurface for å kunne levere med terrengoverflata. Da slipper vegkroppen å ligge i løse lufta.<br /><br />LandSurface er tatt fra LandInfra/Land Feature, men er forenklet kraftig.

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
      <td>geometri</td>
      <td>terrengoverlate i form av en TIN</td>
      <td>GM_<wbr />Tin</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra GenerelleEgenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>Bruker SOSI_Identifikasjon i stedet for LandInfra/ID</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.<br />lokalId skal være en UUID</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- versjon<wbr />Id</td>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans)</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>navn</td>
      <td>Tilsvarer LandInfra/AbstractData/name</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>beskrivelse</td>
      <td>Tilsvarer LandInfra/AbstractData/description</td>
      <td>Character<wbr />String</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
GenerelleEgenskaper

### Kodelister

#### <a id="kodeliste-facilityparttype"></a>«CodeList» FacilityPartType

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td>bridge</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>building</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>drainage</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>environmental</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>railway</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>road</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>site</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>tunnel</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>wastewater</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>waterDistribution</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>other</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-roadelementtype"></a>«CodeList» RoadElementType

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td>pavement</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>pavementSurfaceCourse</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>pavementIntermediateCourse</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>pavementBaseCourse</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>pavementSubbase</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>shoulder</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>hardShoulder</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>softShoulder</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>barrier</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>guardRail</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>curb</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>verticalCurb</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>mountablelCurb</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>curbAndGutter</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>gutter</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>crossPan</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>median</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>greenAreaMedian</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>pavedMedian</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>raisedMedian</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>fencedMedian</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>medianGuardRail</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>medianConcreteBarrier</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>verge</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>sidewalk</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>bikePath</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>drainageDitch</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>cutSlope</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>fillSlope</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>codeList</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-komponentkodesystem"></a>«CodeList» Komponentkodesystem

**Definisjon:** Kodeliste med navn på aktuelle kodesystemer. Lista kan utvides ved behov.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td>HBR761Prosesskode</td>
      <td>Se R761, Prosesskode</td>
      <td></td>
    </tr>
    <tr>
      <td>EPD-ID</td>
      <td>Link (URL) til EPD Norge (eller annen EPD) for oppslag av EPD for aktuell byggevare.</td>
      <td></td>
    </tr>
    <tr>
      <td>NS3420</td>
      <td>NS3420-kode angis tilsvarende denne, som NS-kode med link/URL.:</td>
      <td></td>
    </tr>
    <tr>
      <td>MMI</td>
      <td>Se RIFs Modell Modenhets Indeks for samferdsel</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-dimensjoneringsklasse"></a>«CodeList» Dimensjoneringsklasse

**Definisjon:** Dimensjoneringsklasser for nasjonale hovedveger
Kilde: N100 (versjon mai 2019)

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td>H1</td>
      <td>H1 Nasjonal hovedveg, ÅDT &lt; 6000, fartsgrense 80 km/t</td>
      <td></td>
    </tr>
    <tr>
      <td>H3</td>
      <td>H3 Nasjonal hovedveg, ÅDT &gt; 12000, fartsgrense 110 km/t</td>
      <td></td>
    </tr>
    <tr>
      <td>H5</td>
      <td>H5 Nasjonal hovedveg, ÅDT 6000 -12000, fartsgrense 90 km/t</td>
      <td></td>
    </tr>
    <tr>
      <td>Hø1</td>
      <td>Hø1- Øvrige hovedveger, ÅDT &lt; 4000, fartsgrense 80 km/t</td>
      <td></td>
    </tr>
    <tr>
      <td>Hø2</td>
      <td>Hø2 - Øvrige hovedveger, ÅDT &lt; 120000, fartsgrense 60 km/t</td>
      <td></td>
    </tr>
    <tr>
      <td>L1</td>
      <td>L1 Lokale veger, ÅDT &lt; 1500, fartsgrense 60 km/t eller 80 km/t</td>
      <td></td>
    </tr>
    <tr>
      <td>L2</td>
      <td>L2 Øvrige lokale veger,  ÅDT &lt; 300, lav fartsgrense</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-dimensjonerendehastighet"></a>«CodeList» DimensjonerendeHastighet

**Definisjon:** Dimensjonerende hastighet målt i km/t

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td></td>
      <td>30 km/t</td>
      <td>30</td>
    </tr>
    <tr>
      <td></td>
      <td>40 km/t</td>
      <td>40</td>
    </tr>
    <tr>
      <td></td>
      <td>50 km/t</td>
      <td>50</td>
    </tr>
    <tr>
      <td></td>
      <td>60 km/t</td>
      <td>60</td>
    </tr>
    <tr>
      <td></td>
      <td>80 km/t</td>
      <td>80</td>
    </tr>
    <tr>
      <td></td>
      <td>90 km/t</td>
      <td>90</td>
    </tr>
    <tr>
      <td></td>
      <td>110 km/t</td>
      <td>110</td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-dimensjonerendevegbredde"></a>«CodeList» DimensjonerendeVegbredde

**Definisjon:** Dimensjonerende vegbredde på rettstrekning, dvs. uten hensyn til breddeutvidelse i kurver.
Kilde: N100 (versjon mai 2019)
Kodene er navngitt med m og evt. cm for å unngå at de inneholder kommategn

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td>23m</td>
      <td>23 m</td>
      <td></td>
    </tr>
    <tr>
      <td>12m50cm</td>
      <td>12,5 m</td>
      <td></td>
    </tr>
    <tr>
      <td>9m</td>
      <td>9 m</td>
      <td></td>
    </tr>
    <tr>
      <td>7m50cm</td>
      <td>7,5 m</td>
      <td></td>
    </tr>
    <tr>
      <td>6m</td>
      <td>6 m</td>
      <td></td>
    </tr>
    <tr>
      <td>4m</td>
      <td>4 m</td>
      <td></td>
    </tr>
    <tr>
      <td>3m50cm</td>
      <td>3,5 m</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-dimensjonerendemotorkjøretøy"></a>«CodeList» DimensjonerendeMotorkjøretøy

**Definisjon:** Dimensjonerende motorkjøretøy velges ut fra veg-og gatenettets funksjon, trafikkmengde og muligheterfor omkjøring.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td>P</td>
      <td>Personbiler, varebiler, kombibiler (P)</td>
      <td></td>
    </tr>
    <tr>
      <td>LL</td>
      <td>Liten lastebil (LL)</td>
      <td></td>
    </tr>
    <tr>
      <td>L</td>
      <td>Lastebiler (inkl. brannbiler med stige) (L)</td>
      <td></td>
    </tr>
    <tr>
      <td>B</td>
      <td>Boggibusser (B)</td>
      <td></td>
    </tr>
    <tr>
      <td>VT</td>
      <td>Vogntog (VT)</td>
      <td></td>
    </tr>
    <tr>
      <td>MVT</td>
      <td>Modulvogntog (MVT)</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-dimensjonerendetrafikkmengdeådt"></a>«CodeList» DimensjonerendeTrafikkmengdeÅDT

**Definisjon:** Dimensjonerende antall kjøretøy i snitt pr døgn, ÅDT

Kilde: N100 (versjon mai 2019)
<a href="https://www.vegvesen.no/siteassets/content/vedlegg/handboker/n100-veg-og-gateutforming-041219.pdf">https://www.vegvesen.no/siteassets/content/vedlegg/handboker/n100-veg-og-gateutforming-041219.pdf</a>

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td>under6000</td>
      <td>&lt;6000 kjøretøy i snitt pr døgn</td>
      <td></td>
    </tr>
    <tr>
      <td>mellom6000og12000</td>
      <td>6000-12000  kjøretøy i snitt pr døgn</td>
      <td></td>
    </tr>
    <tr>
      <td>over12000</td>
      <td>&gt;12000 kjøretøy i snitt pr døgn</td>
      <td></td>
    </tr>
    <tr>
      <td>under4000</td>
      <td>&lt;4000 kjøretøy i snitt pr døgn</td>
      <td></td>
    </tr>
    <tr>
      <td>under12000</td>
      <td>&lt;12000 kjøretøy i snitt pr døgn</td>
      <td></td>
    </tr>
    <tr>
      <td>under1500</td>
      <td>&lt;1500 kjøretøy i snitt pr døgn</td>
      <td></td>
    </tr>
    <tr>
      <td>under300</td>
      <td>&lt;300 kjøretøy i snitt pr døgn</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-dimensjonerendekjøremåte"></a>«CodeList» DimensjonerendeKjøremåte

**Definisjon:** Beskriver den frihet et kjøretøy trenger i veg-/kjørearealet ved trafikkering av vegnettet. Se kjøremåte A, B og C.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td>A</td>
      <td>Kjøremåte A:
Ved kjøremåte A forutsettes følgende nårdet gjelder dimensjonerende kjøretøy:
&lt;ul&gt;
&lt;li&gt;kjøretøyet skal kunne trafikkere veg-/gateanlegget kun ved bruk av eget kjørefelt. Dette betyr athele kjøretøyet, inklusiv overheng, skal kunne bevege seg innenfor sitt eget kjørefelt&lt;/li&gt;
&lt;li&gt;på veger og gater utenom kryss skal disse strekningene kunne trafikkeres med en fart tilsvarendefartsgrensen&lt;/li&gt;
&lt;li&gt;i kryss skal kjøretøyet kunne kjøre gjennom krysset med en fart på 15 km/t&lt;/li&gt;
&lt;li&gt;i slyng skal kjøretøyet kunne kjøre med en fart på 15 km/t&lt;/li&gt;
&lt;/ul&gt;
&lt;ul&gt;
&lt;li&gt;kjøretøyet skal ikke behøve å rygge på snuplasser&lt;/li&gt;
&lt;/ul&gt;</td>
      <td></td>
    </tr>
    <tr>
      <td>B</td>
      <td>Kjøremåte B:
Ved kjøremåte B forutsettes følgende når det gjelder dimensjonerende kjøretøy:
&lt;ul&gt;
&lt;li&gt;i kryss forutsettes kjøretøyet å kunne bruke deler av motgående kjørefelt i den veg/gate kjøretøyetsvinger inn i&lt;/li&gt;
&lt;li&gt;på veger og gater utenfor kryss antas at valgt kjøretøy på enkelte partier trafikkerer disse med enlavere fart enn fartsgrensen&lt;/li&gt;
&lt;li&gt;i kryss forutsettes valgt kjøretøy å kunne kjøre gjennom krysset med en lavere fart enn 15 km/t&lt;/li&gt;
&lt;li&gt;i slyng skal kjøretøyet kunne kjøre med en fart på 15 km/t&lt;/li&gt;
&lt;li&gt;kjøretøyet vil i noen tilfeller måtte regne med å rygge på snuplasser&lt;/li&gt;
&lt;/ul&gt;</td>
      <td></td>
    </tr>
    <tr>
      <td>C</td>
      <td>Kjøremåte C:
Kjøremåte C vil primært være knyttet til kryss. Ved kjøremåte C forutsettes følgende når det gjelder dimensjonerende kjøretøy:
&lt;ul&gt;
&lt;li&gt;kjøretøyet forutsettes å kunne bruke hele kjørebanebredden både i den veg/gate kjøretøyet svinger av fra og i den veg/gate kjøretøyet svinger inn i&lt;/li&gt;
&lt;li&gt;valgt kjøretøy forutsettes å kjøre gjennom krysset med en lavere fart enn 15 km/t&lt;/li&gt;
&lt;li&gt;kjøretøyet vil i noen tilfeller måtte regne med å rygge på snuplasser&lt;/li&gt;
&lt;/ul&gt;</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-maxoverhøydeprosent"></a>«CodeList» MaxOverhøydeProsent

**Definisjon:** Max tverrfall/overhøyde målt i prosent
Kilde N100 (versjon mai 2019)

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td></td>
      <td>8 %</td>
      <td>8</td>
    </tr>
    <tr>
      <td></td>
      <td>5 %</td>
      <td>5</td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-dimensjonerendetrafikkgruppe"></a>«CodeList» DimensjonerendeTrafikkgruppe

**Definisjon:** Trafikkgruppe målt i ekvivalente 10 tonns aksler (N):
Dimensjonerende aksellast: 10 tonn
Dimensjoneringsperiode: 20 år
Dimensjonerende trafikkbelastning: Ekvivalente 10 tonns aksler per felt i dimensjoneringsperioden.
Kilde: N200 (2018)

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td>A</td>
      <td>&lt;500 000 = Trafikkgruppe A</td>
      <td></td>
    </tr>
    <tr>
      <td>B</td>
      <td>500 000 - 1 000 000 = Trafikkgruppe B</td>
      <td></td>
    </tr>
    <tr>
      <td>C</td>
      <td>1 000 000 – 2 000 000 = Trafikkgruppe C</td>
      <td></td>
    </tr>
    <tr>
      <td>D</td>
      <td>2 000 000 – 3 500 000 = Trafikkgruppe D</td>
      <td></td>
    </tr>
    <tr>
      <td>E</td>
      <td>3 500 000 – 10 000 000 = Trafikkgruppe E</td>
      <td></td>
    </tr>
    <tr>
      <td>F</td>
      <td>&gt; 10 000 000 = Trafikkgruppe F</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-overbygninglagtype"></a>«CodeList» OverbygningLagtype

**Definisjon:** Kodeliste som betegner fysisk lag i overbygningen

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td>slitelag</td>
      <td>Det øverste laget i et vegdekke. Settes sammen/beregnes for å kunne oppta trafikk- og klimapåkjenninger.</td>
      <td></td>
    </tr>
    <tr>
      <td>bindelag</td>
      <td>Nedre del av asfaltdekket når dette består av mer enn ett lag, dvs. lag mellom slitelag og bærelag.</td>
      <td></td>
    </tr>
    <tr>
      <td>bærelag</td>
      <td>Bærelag. Dersom det brukes flere bærelag, skilles de med lagnummer.</td>
      <td></td>
    </tr>
    <tr>
      <td>forsterkningslag</td>
      <td>Lag i vegens overbygning, under bærelag. Hovedfunksjonen er å fordele trafikkbelastningen slik at undergrunnen ikke overbelastes.</td>
      <td></td>
    </tr>
    <tr>
      <td>frostsikringslag</td>
      <td>Lag under forsterkningslaget, eller bygget sammen med forsterkningslaget, for å hindre frosten i å trenge ned i tele- farlig undergrunn eller underbygning.</td>
      <td></td>
    </tr>
    <tr>
      <td>filterlag</td>
      <td>Lag av filtermateriale, normalt nederste lag i overbygningen mellom planum og forsterkningslaget. Er i dag normalt erstattet av en fiberduk.</td>
      <td></td>
    </tr>
    <tr>
      <td>fiberduk</td>
      <td>Kan være fiberduk. Fiberduk kan legges under armeringslaget for å unngå at materialer fra grunnen trenger inn i overbygningen.</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-side"></a>«Enumeration» Side

**Definisjon:** kodeliste for angivelse av vegside

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
      <td>left</td>
      <td>venstre side</td>
      <td></td>
    </tr>
    <tr>
      <td>right</td>
      <td>høyre side</td>
      <td></td>
    </tr>
    <tr>
      <td>both</td>
      <td>begge sider</td>
      <td></td>
    </tr>
    <tr>
      <td>neither</td>
      <td>ingen av sidene</td>
      <td></td>
    </tr>
    <tr>
      <td>unspecified</td>
      <td>uspesifisert side</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-underbygninglagtype"></a>«CodeList» UnderbygningLagtype

**Definisjon:** Kodeliste som betegner fysisk lag i underbygningen

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
  </tbody>
</table>

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
      <td>undergrunn</td>
      <td>Eksisterende masser i grunnen, som gjennom bearbeiding, evt. ved tilsetning av materialer, får en forbedret styrke i forhold til opprinnelig styrke. Eksempler på tiltak kan være komprimering, senking av grunnvannstanden. Formålet er å oppnå en redusert tykkelse på nødvendig overbygning. Se også grunnforsterkning med lokale materialer.</td>
      <td></td>
    </tr>
    <tr>
      <td>dypsprengning</td>
      <td>Løssprengning av fjell til et visst nivå under teoretisk traubunn.</td>
      <td></td>
    </tr>
    <tr>
      <td>undergrunnForbedret</td>
      <td>Eksisterende masser i grunnen som er forbedret eller stabilisert</td>
      <td></td>
    </tr>
    <tr>
      <td>fylling</td>
      <td>Fylling som del av underbyggning</td>
      <td></td>
    </tr>
  </tbody>
</table>
