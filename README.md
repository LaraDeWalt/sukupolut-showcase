# Sukupolut

**Source-based genealogy, connected through people, places and stories.**

Sukupolut is a Finnish-language research application that brings historical records, family relationships, places and narrative material into one connected workspace. It preserves source observations and uncertainty instead of hiding the evidence behind a single family-tree conclusion.

## The problem

The same person may appear under different names, dates and households across historical records. Places and their administrative relationships also change over time. Researchers need to compare evidence, correct interpretations and understand who lived where and when.

Sukupolut keeps people, source observations and research interpretations distinct, while connecting them through searchable profiles, family trees, maps and household views.

## What works today

### Source-based research
- Source-specific entry forms for historical Finnish records, including population, communion, children's, birth, death and migration records.
- Source references, original observations and uncertain or conflicting information retained alongside structured data.
- GEDCOM import with review, decisions to create or merge people, and import provenance.
- Duplicate-person and duplicate-place merging with linked observations retained.
- Source links and source-linked observations connected to people and places.

### People and families
- Person profiles with life events, relationships, place connections, photographs and related stories.
- Expandable family-tree views with search, zoom and fit controls.
- Profile actions for adding relatives, linking a place, writing a person's story and attaching photographs or newspaper clippings.
- Profile-photo cropping and an image viewer.
- Separate editing controls for basic information, duplicate merging and person deletion.

### Places and households
- Place hierarchies, historical place observations and map locations.
- Place pages connecting descriptions, photographs, stories, related places and research links.
- Year-based house views grouping recorded residents into households and showing their family relationships.
- Source-based entry directly from a house, croft or village page, including cases where the source names only a village.
- Distinct treatment of recorded residence and place of death.
- Grayscale map backgrounds with clearer labels for saved research locations.

### Stories and research interface
- A newspaper-inspired home view organised around families, stories and places.
- Stories, photographs and newspaper clippings connected to people, multiple places and dates or periods.
- Year-based browsing of narrative material.
- Saved family-branch shortcuts and photograph-led home-page selections.
- More accessible profile workflows and subtly rounded interface controls.

### Accounts and local operation
- SQLite storage and a browser-based interface.
- Application accounts with viewer, editor and administrator roles, personal invitations and server-side permission checks.
- A shared research dataset for authorised users; accounts do not create isolated family databases.
- Backup tooling and deployment configuration for a future shared test service.

## Recent development

The November updates have expanded the original record-entry prototype into a connected research interface:

- **Research context:** household views, historical place connections and family-tree navigation.
- **Narrative material:** stories, photographs and newspaper clippings linked to research subjects.
- **Data quality:** reviewed GEDCOM import, duplicate merging and explicit distinctions between different kinds of place evidence.
- **Everyday usability:** direct entry from person and place pages, clearer editing controls and improved map readability.

## Technical approach

| Area | Implementation |
| --- | --- |
| Backend | Python, local HTTP server and a WSGI entry point |
| Database | SQLite with relational links and source observations |
| Interface | HTML, CSS and JavaScript |
| Maps | Leaflet |
| Data model | People and places separated from source-specific observations |
| Access control | Application accounts and server-side role checks |
| Verification | Python and JavaScript tests covering data operations and interface behaviour |

## My contribution

I have driven the project from identifying research needs and defining requirements to designing the data model, shaping the interface, developing a prototype with AI assistance and iterating through testing and practical research workflows.

The project demonstrates:
- translating complex domain workflows into structured requirements and usable forms;
- relational data modelling and traceable handling of inconsistent evidence;
- identifying quality risks and defining validation and correction workflows;
- connecting structured information to visual, user-centred research tools;
- continuous improvement based on real usage.

## Project status

**Working prototype, actively developed. Overview updated 16 November 2026, based on the application package dated 13 November 2026.**

The application runs locally. Accounts and deployment preparation are implemented, but a shared hosted service has not been launched. Payment integration and a certification course are not implemented.

The application source code and research material remain private. This public repository is a project overview and contains no research database, personal records, credentials or private application source code.

## Suomeksi

Sukupolut on kehitteillä oleva lähdepohjainen sukututkimussovellus, joka yhdistää henkilöt, suvut, paikat ja tarinat. Keskeistä on tiedon alkuperän säilyttäminen: lähdehavainnot ja tutkijan tulkinnat erotetaan toisistaan, ja epävarmuuksia voidaan tarkastella.

Sovelluksessa on muun muassa lähdekohtainen aineistonsyöttö, tarkistettava GEDCOM-tuonti, henkilöprofiilit ja sukupuut, kartat ja historialliset paikkayhteydet sekä talojen vuosittaiset perhekuntanäkymät. Tarinoita, valokuvia ja lehtileikkeitä voi liittää henkilöihin ja paikkoihin. Uusimmat muutokset helpottavat tietojen lisäämistä suoraan henkilö- ja paikkasivuilta.

Olen vienyt projektia tarpeen tunnistamisesta ja vaatimusmäärittelystä tietomallin ja käyttöliittymän suunnitteluun, tekoälyavusteiseen prototyypin kehittämiseen ja testaukseen. Projekti havainnollistaa erityisesti kokonaisuuksien hahmottamista, tiedon laadunvarmistusta ja käytännönläheistä prosessien kehittämistä.

**Created by [Laura Paasonen](https://github.com/LaraDeWalt).**
