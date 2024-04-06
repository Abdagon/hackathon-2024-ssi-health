https://www.youtube.com/watch?v=uNrMFE2wOyQ

**\*\*\* [English version](#english) below \*\*\***

**Nutzung von verifiable credentials für vertrauenswürdige strukturierte Gesundheitsdaten**

![Gesundheitsdaten im persönlichen digitalen Wallet](https://bucketeer-036aa605-c047-4623-8610-f1764b90cf98.s3.amazonaws.com/public/374/GLC9QNEXBDU1A79TEYHVUK8D/Health_Data_in_Wallet.jpg)
Erzeugt mit Dall-E 3, prompt «person-centric wallet-based structured healthcare data»

# Challenge

Mit dem Challenge soll als «Proof of Concept» (PoC) ein Anwendungsfall mit Gesundheitsdaten als «Showcase» umgesetzt werden, basierend auf der SSI-basierten Vertrauens-Infrastruktur der neuen Schweizer E-ID.

Der Vorteil der Vertrauens-Infrastruktur gegenüber aktuellen zentralisierten Ansätzen ist die personenzentrierte, sichere und vertrauenswürdige Speicherung der Gesundheitsdaten in der persönlichen digitalen Wallet (siehe [DIDAS Statement for E-ID Technology Discussion Paper](https://www.didas.swiss/2024/02/21/4478/)).

Die Daten liegen dadurch beim Bürger und können ohne seinen Konsent nicht durch Dritte eingesehen werden. Die Technologie der Vertrauens-Infrastruktur ermöglicht, den Fokus auf fachliche Themen zu legen.

Dieser Challenge bietet Interessierten die Möglichkeit, sich früh mit Konzepten und Technologien vertraut zu machen, welche die Grundlage für E-IDs und viele weitere sichere Anwendungen bildet, und für welche sich eine zunehmende Nachfrage entwickelt.

https://www.youtube.com/watch?v=z5URtBhYSMY

Challenge Pitch Video (YouTube)

## Ressourcen

Die neue [E-ID der Schweiz](https://www.ejpd.admin.ch/bj/de/home/staat/gesetzgebung/staatliche-e-id.html) basiert auf den Prinzipien der [Self Sovereign Identity](https://en.wikipedia.org/wiki/Self-sovereign_identity#:~:text=Self%2Dsovereign%20identity%20(SSI),and%20applications%20across%20the%20web.) (SSI), die Einführung ist für 2026 geplant. Für die E-ID wird aktuell ein [Ökosystem](https://github.com/e-id-admin) mit einer Vertrauens-Infrastruktur (trust infrastructure) aufgebaut. Die Möglichkeiten dieses Ökosystems gehen weit über die E-ID hinaus - Prinzipien und Technologie lassen sich in unterschiedlichen Sektoren wie Gesundheitswesen, Finanzwesen, Mobilität, Logistik, etc. nutzen. Um möglichst früh praktische Erfahrungen zu sammeln, steht eine [E-ID Sandbox](https://github.com/e-id-admin/public-sandbox-trustinfrastructure) zur Verfügung.

Der Verein [DIDAS](https://www.didas.swiss/) engagiert sich in der Schweiz für die Förderung von SSI Prinzipien und Umsetzungen. In [Arbeitsgruppen](https://www.didas.swiss/working-groups/) werden Themen der verschiedenen Sektoren bearbeitet.

![Check-in für Patient](https://bucketeer-036aa605-c047-4623-8610-f1764b90cf98.s3.amazonaws.com/public/374/KJLGB9RVTFIOHOJUGQHRDQBD/Patient_Checkin.jpg)
Erzeugt mit Dall-E 3, prompt «digital patient check-in to doctor's office reception desk with QR-code»

Der [Anwendungsfall](https://github.com/janesp/health-ssi) (Use Case) für den Challenge ist ein Arzttermin unter Nutzung der Möglichkeiten der Vertrauens-Infrastruktur:

* Der Patient John Miller verfügt über eine Wallet mit Informationen seiner Gesundheitsdaten (Allergien, Medikamente, etc.) sowie einer Versicherungskarte in Form von vorgängig ausgestellten Verifiable Credentials.
* John betritt die Praxis von Dr. Charles Brewster und meldet sich über einen QR-Code an; dadurch wird eine Abfrage von Versicherungs- und Gesundheitsinformationen in Johns Wallet ausgelöst (proof request), welche von John bestätigt wird.
* Dr. Brewster stellt im Rahmen der Konsultation die Ergebnisse seiner Untersuchung als Verifiable Credentials aus und verschreibt einige Medikamente, ebenfalls in Form von Verifiable Credentials.
* Nach der Visite bestellt John die Medikamente über den Online-Shop «Universal Pharmacy» unter Vorlage des Rezeptes als Verifiable Credentials.

Für den Challenge steht für rasches Prototyping eine Umgebung analog zur E-ID Sandbox zur Verfügung.
Als Abstraktion von der aktuellen Technologie der E-ID Sandbox wird das [Verifiable Credential Management System](https://github.com/SSI-Solutions/vcms/tree/main) (VCMS) genutzt.
Für medizinische Informationen werden im Interesse der Interoperabilität internationale Standards verwendet:

* [FHIR](http://www.hl7.org/fhir/), Teil der Standards von [HL7](http://www.hl7.org/)
* [FHIR.ch](http://www.fhir.ch/), Schweizer Spezifika
* [International Patient Summary](https://international-patient-summary.net/) (IPS)
* [openEHR](https://openehr.org/)
* [SNOMED CT](https://www.snomed.org/)

Für Themen der digitalen Transformation im Gesundheitswesen bestehen zudem interessante Podcasts und Webinare:

* [Marktplatz Gesundheitswesen](https://gesundheitswesen.org/) (CH) - ZHAW, Prof. Dr. Alfred Angerer
* [eHealth-Podcast](https://www.ehealth-podcast.de/) (DE) - DER Podcast rund um Gesundheits- und Medizininformatik, Hochschulen Konstanz und Niederrhein
* [e-Health Pioneers Podcast](https://themedicalnetwork.de/podcast/) (DE) - The Medical Network, Andrea Buzzi
* [DIDAS Health Webinare](https://www.youtube.com/playlist?list=PLDiii1ZjtiLbqqg1OYZ8dakz6yLpitenf) (CH/EU) - Aufzeichnungen von Gastreferaten

Für die technische Umsetzung können im Sinne eines raschen Prototypings Frameworks verwendet werden, z.B.

* [strapi](https://strapi.io/) \- modernes «headless» CMS
* [Drupal](https://www.drupal.org/) \- mächtiges CMS \(mit steiler Lernkurve\)\, «headless» verfügbar
* [Svelte](https://svelte.dev/), [SvelteKit](https://kit.svelte.dev/) \- Komponenten und Framework für Web Apps
* [Verifiable Credentials Playground](https://vcplayground.org), inkl. [chapi](https://chapi.io) Dokumentation
* …

## Goal

Im Challenge soll der Anwendungsfall mit den persönlichen Gesundheitsdaten als «Showcase» PoC umgesetzt werden, basierend auf der SSI-basierten Vertrauens-Infrastruktur der neuen Schweizer E-ID.

Dafür sollen Prototypen der einzelnen Komponenten entwickelt bzw. konfiguriert werden:

* Wallet des Patienten John Miller, vorbereiteten Verifiable Credentials für Versicherungskarte und Allergien (Holder und Verifier Rolle)
* Relevante Elemente des Praxis-Informationssystems von Dr. Brewster
    * Allergien aus IPS (Verifier Rolle)
    * Anamnese, Diagnose, Medikation für die Erstellung von Verifiable Credentials (Issuer Rolle)
* Relevante Elemente der Versand-Apotheke «Universal Pharmacy» (Verifier Rolle)

Für die Umsetzung werden basierend auf den internationalen Standards Schemas für die benötigten Verifiable Credentials definiert.
Mit dem Front-End der Prototypen werden die relevanten Datenobjekte erfasst und visualisiert, ein Teil des Back-Ends erstellt damit über VCMS-Aufrufe die jeweiligen Verifiable Credentials.

## Outcomes

Der SSI Health PoC Showcase dient dazu, im Jahr 2024 fachlichen und technischen Interessengruppen aufzuzeigen, wie SSI-Prinzipien sowie die Vertrauens-Infrastruktur für strukturierte und vertrauenswürdige Gesundheitsdaten genutzt werden können.

Basierend auf dieser Sensibilisierung wird angestrebt, mit der Einführung der E-ID 2026 darauf basierende Anwendungsfälle zu zeigen und ggf. bereits anzubieten.

Es ist vorgesehen, vom Ergebnis des Hackathons neben der geplanten Dokumentation ein kurzes Video zu erstellen (z.B. wie für den [OnceHealth PoC](https://youtu.be/T5bYmy_oXMo)), welches Interessenten gezeigt werden kann.

## Solutions

Für die digitale Transformation im Gesundheitswesen gibt es eine Vielzahl von Initiativen, jedoch bisher mit beschränktem Erfolg; nachfolgend sind exemplarisch einige davon aufgeführt:

* [Elektronisches Patientendossier](https://www.patientendossier.ch/privatpersonen) (EPD) - basierend auf unstrukturierten PDF-Dokumenten, einige 100 M CHF Kosten über die letzten 10 Jahre, aktuell etwa 20’000 eröffnete Dossiers
* [Well](https://www.well.ch/) \- Angebot der Versicherer\, keine Integration des EPD
* [Compassana](https://www.compassana.ch/) \- Angebot der Versicherer\, keine Integration des EPD
* HealthLink - Initiative der ehemaligen axsana
* OnceHealth - [Prototyp](https://youtu.be/T5bYmy_oXMo), [Positionierung](https://drive.google.com/drive/folders/1rjdld14PXWpas2VALUmgrYFgNeRXBS0B)
* openEHR PoC und Ausschreibung des Universitätsspitals Basel
* [openEHR.ch](https://openehr.ch/) \- Schweizer Verein als Teil der globalen Organisation [openEHR.org](https://openehr.org/)
* [Cobedias](https://www.cobedix.ch/) \- strukturierte Erfassung von Gesundheitsdaten für niedergelassene Ärzte
* [Gesundheitsdatenraum Schweiz](https://gesundheitsdatenraum.ch/)
* [HIN SSI Proof of Concept](https://youtu.be/PTWGwz9Sd7U) für ärztliche Berufsausübungsbewilligungen (BAB)
* …

Die Mehrheit dieser Initiativen strebt strukturierte Gesundheitsdaten an, keine davon ausser dem HIN SSI PoC orientiert sich jedoch an SSI-Prinzipien.

## Restrictions

SSI Technologien sind aktuell noch nicht vollständig bereit für produktive Einsätze, viele Aspekte sind noch im Wandel.

Die Technologie der für die 2026 geplanten E-ID ist aktuell noch nicht entschieden (siehe [DIDAS Statement for E-ID Technology Discussion Paper](https://www.didas.swiss/2024/02/21/4478/)).

Die aktuelle E-ID Sandbox wird basierend auf dem in Kürze erwarteten E-ID Technologie-Entscheid auf diese neue Technologie migriert (Sandbox 2.0). Es ist vorgesehen, VCMS ebenfalls auf diese neue Technologie zu migrieren.

## Verwendung

Mit dem «Showcase» PoC des konkreten Anwendungsfalls sollen mehrere Ziele erreicht werden, indem konkrete Möglichkeiten demonstriert werden:

* Machbarkeit der Nutzung der Vertrauens-Infrastruktur und Verifiable Credentials für strukturierte und vertrauenswürdige Gesundheitsdaten
* Zusammenspiel verschiedener Beteiligter wie Bürger, Arzt und Apotheke im Ökosystem der Vertrauens-Infrastruktur
* Konkreter fachlicher Anwendungsfall als Demonstrator der DIDAS Health Arbeitsgruppe
* Konkreter fachlicher (nicht technischer) Anwendungsfall für die SSI-Community, z.B. Vorstellung an der [DICE 2024](https://diceurope.org/)
* Verbesserung semantischer Interoperabilität von strukturierten und standardisierten Gesundheitsdaten zum Nutzen von Bürgern und Leistungserbringern

Mögliche Weiterentwicklungen der aktuellen Gesundheitsdaten-Infrastruktur als Sensibilisierung für Vertreter des Gesundheitswesens (siehe auch [DIDAS Stellungnahme zur Vernehmlassung EPDG](https://www.didas.swiss/de/2023/11/13/didas-stellungnahme-zur-epdg-revision/)) - besserer und sicherer Datenaustausch, weniger Papier, weniger Umkopieren, raschere Prozesse, bessere Behandlungen, weniger Komplikationen, weniger Administration

## Organisation

* Abdagon AG, Dr. Peter Janes, Founder and CEO; DIDAS Health Lead
* Adnovum AG, Dr. Roman Zoun, Head Security Solutions Offerings; DIDAS Adoption Lead
* DIDAS

## Weitere Information

* Breaking News 29.02.2024, Europäisches Parlament nimmt eIDAS 2.0 an - [MEPs back plans for an EU-wide digital wallet](https://www.europarl.europa.eu/news/en/press-room/20240223IPR18095/meps-back-plans-for-an-eu-wide-digital-wallet)
* [EU Health Data Space must be individual-centric to benefit all stakeholders](https://mydata.org/2023/12/13/eu-health-data-space-must-be-individual-centric-to-benefit-all-stakeholders/)
* ...

***

<br>
<br>
**\*\*\* English version \*\*\***

# Digital Health with the new E-ID trust infrastructure

## Using verifiable credentials for trustworthy structured healthcare data

![Healthcare data in the personal digital wallet](https://bucketeer-036aa605-c047-4623-8610-f1764b90cf98.s3.amazonaws.com/public/374/GLC9QNEXBDU1A79TEYHVUK8D/Health_Data_in_Wallet.jpg)
Generated with Dall-E 3, prompt «person-centric wallet-based structured healthcare data»

# Challenge

This challenge aims to implement a proof of concept (PoC) use case with healthcare data as a showcase, based on the SSI trust infrastructure of the new Swiss E-ID.

The advantage of the trust infrastructure over current centralized approaches is the person-centered, secure and trustworthy storage of health data in the personal digital wallet (see [DIDAS Statement for E-ID Technology Discussion Paper](https://www.didas.swiss/2024/02/21/4478/)).

This means that the data remains with the citizen and cannot be viewed by third parties without their consent. The technology of the trust infrastructure makes it possible to focus on specialist topics.

This challenge offers interested participants the opportunity to familiarize themselves early on with concepts and technologies that form the basis for E-IDs and many other secure applications and for which there is increasing demand.

## Resources

[Switzerland's new e-ID](https://www.ejpd.admin.ch/bj/de/home/staat/gesetzgebung/staatliche-e-id.html) is based on the principles of [Self Sovereign Identity](https://en.wikipedia.org/wiki/Self-sovereign_identity#:%7E:text=Self%2Dsovereign%20identity%20(SSI),and%20applications%20across%20the%20web.) (SSI) and is scheduled for introduction in 2026. An ecosystem with a trust infrastructure is currently being set up for the E-ID. The possibilities of this ecosystem go far beyond the E-ID – principles and technology can be used in various sectors such as healthcare, finance, mobility, logistics, etc. An [E-ID Sandbox](https://github.com/e-id-admin/public-sandbox-trustinfrastructure) is available to gather practical experience as early as possible.

The [DIDAS](https://www.didas.swiss/) association is committed to promoting SSI principles and implementation in Switzerland. Topics from the various sectors are dealt with in [working groups](https://www.didas.swiss/working-groups/).
 
![Check-in for patient](https://bucketeer-036aa605-c047-4623-8610-f1764b90cf98.s3.amazonaws.com/public/374/KJLGB9RVTFIOHOJUGQHRDQBD/Patient_Checkin.jpg)
Generated with Dall-E 3, prompt «digital patient check-in to doctor's office reception desk with QR-code»

The [use case](https://github.com/janesp/health-ssi) for this challenge is a doctor's appointment using the possibilities of the trust infrastructure:

* The patient John Miller has a digital wallet with information about his health data (allergies, medication, etc.) as well as an insurance card in the form of previously issued verifiable credentials.
* John enters Dr. Charles Brewster's office and checks in using a QR code; this triggers a request for insurance and health information in John's wallet (proof request), which John confirms.
* During the consultation, Dr. Brewster issues the results of his examination as verifiable credentials and prescribes some drugs, also in the form of verifiable credentials.
* After the visit, John orders the drugs via the online store «Universal Pharmacy», presenting the prescription as verifiable credentials.

For this challenge, an environment similar to the E-ID Sandbox is available for rapid prototyping. The [Verifiable Credential Management System](https://github.com/SSI-Solutions/vcms/tree/main) (VCMS) is used as an abstraction of the current E-ID Sandbox technology. International standards are used for medical information in the interests of interoperability:

* [FHIR](http://www.hl7.org/fhir/), part of the [HL7](http://www.hl7.org/) standards
* [FHIR.ch](http://www.fhir.ch/), Swiss specifics
* [International Patient Summary](https://international-patient-summary.net/) (IPS)
* [openEHR](https://openehr.org/)
* [SNOMED CT](https://www.snomed.org/)

There are also interesting podcasts and webinars on topics relating to digital transformation in the healthcare sector:

* [Marktplatz Gesundheitswesen](https://gesundheitswesen.org/) (CH, German) – ZHAW, Prof. Dr. Alfred Angerer
* [eHealth Podcast](https://www.ehealth-podcast.de/) (DE, German) – DER Podcast rund um Gesundheits- und Medizininformatik, Hochschulen Konstanz und Niederrhein
* [e-Health Pioneers Podcast](https://themedicalnetwork.de/podcast/) (DE, German) – The Medical Network, Andrea Buzzi
* [DIDAS Health Webinars](https://www.youtube.com/playlist?list=PLDiii1ZjtiLbqqg1OYZ8dakz6yLpitenf) (CH/EU, English) – Recordings of guest presenters

Frameworks can be used for the technical implementation in the sense of rapid prototyping, e.g.

* [strapi](https://strapi.io/) – modern «headless» CMS
* [Drupal](https://www.drupal.org/) – powerful CMS (with a steep learning curve), supports «headless»
* [Svelte](https://svelte.dev/), [SvelteKit](https://kit.svelte.dev/) – components and framework for web apps
* [Verifiable Credentials Playground](https://vcplayground.org/), incl. [chapi](https://chapi.io/) documentation
* ...

## Goal

In this challenge, the use case with the personal health shall be implemented as a «showcase» PoC, based on the SSI trust infrastructure of the new Swiss E-ID.

To this end, prototypes of the individual components shall be developed and configured:

* Wallet of the patient John Miller, prepared verifiable credentials for insurance card and allergies (holder and verifier role)
* Relevant elements of Dr. Brewster's practice information system
* Allergies from IPS (verifier role)
* Medical history, diagnosis, medication for the creation of verifiable credentials (issuer role)
* Relevant elements of the mail-order pharmacy «Universal Pharmacy» (verifier role)

Schemas for the required verifiable credentials are defined for implementation based on international standards. The relevant data objects are stored and visualized with the front end of the prototypes, and part of the back end uses them to create the respective verifiable credentials via VCMS calls.

## Outcomes

The SSI Health PoC Showcase serves to demonstrate to healthcare and technical stakeholders in 2024 how SSI principles and the trust infrastructure can be used for structured and trustworthy healthcare data.

Based on this growing awareness, the aim is to demonstrate use cases based with the introduction of the E-ID in 2026 and, if necessary, to offer them already.

In addition to the envisaged documentation, it is planned to create a short video of the result of the hackathon (e.g. as for the [OnceHealth PoC](https://youtu.be/T5bYmy_oXMo)), which can be shown to interested stakeholders.

## Solutions

There are a number of initiatives for digital transformation in the healthcare sector, albeit with limited success to date; some of these are listed below as examples:

* [Electronic patient record](https://www.patientrecord.ch/individuals) (EPR) – based on unstructured PDF documents, costs of several 100 M CHF over the last 10 years, currently around 20,000 opened dossiers
* [Well](https://www.well.ch/en/) – offered by health insurance companies, no integration of the EPR
* [Compassana](https://www.compassana.ch/en) – offered by health insurance companies, no integration of the EPR
* HealthLink – initiative of the former axsana
* OnceHealth – [prototype](https://youtu.be/T5bYmy_oXMo), [positioning](https://drive.google.com/drive/folders/1rjdld14PXWpas2VALUmgrYFgNeRXBS0B)
* openEHR PoC and request for proposal of the University Hospital Basel
* [openEHR.ch](https://openehr.ch/) – Swiss association as Swiss branch of the global organization openEHR.org
* [Cobedias](https://www.cobedix.ch/en) – structured recording of health data for registered doctors
* [Swiss Health Data Space](https://gesundheitsdatenraum.ch/en/)
* [HIN SSI Proof of Concept](https://youtu.be/PTWGwz9Sd7U) for medical practice licenses (BAB)
* ...

The majority of these initiatives aim for structured health data, but none of them except the HIN SSI PoC are based on SSI principles.

## Restrictions

SSI technologies are not yet fully ready for productive use, many aspects are still emerging.

The technology of the E-ID planned for 2026 has not yet been decided (see [DIDAS Statement for E-ID Technology Discussion Paper](https://www.didas.swiss/2024/02/21/4478/)).

The current E-ID sandbox will be migrated to this new technology based on the E-ID technology decision expected shortly (Sandbox 2.0). It is planned to migrate VCMS to this new technology as well.

## Usage

The «showcase» PoC of this specific use case is intended to achieve several objectives by demonstrating specific possibilities:

* Feasibility of using the trust infrastructure and verifiable credentials for structured and trusted healthcare data
* Interaction between various stakeholders such as citizens, medical doctors and pharmacies in the trust infrastructure ecosystem
* Specific healthcare use case as a demonstrator of the DIDAS Health working group
* Specific healthcare (non-technical) use case for the SSI community, e.g. presentation at [DICE 2024](https://diceurope.org/)
* Improving semantic interoperability of structured and standardized health data for the benefit of citizens and service providers

Possible further development of the current health data infrastructure to increase awareness among representatives of the healthcare sector (see also [DIDAS statement on the EPDG consultation](https://www.didas.swiss/2023/11/13/didas-statement-on-the-epdg-revision/)) – better and secure data exchange, less paper, less copying, faster processes, better treatments, fewer complications, less administration

## Organization

* Abdagon AG, Dr. Peter Janes, Founder and CEO; DIDAS Health Lead
* Adnovum AG, Dr. Roman Zoun, Head Security Solutions Offerings; DIDAS Adoption Lead
* DIDAS

## Further information

* Breaking News 29.02.2024, European Parliament adopts eIDAS 2.0 – [MEPs back plans for an EU-wide digital wallet](https://www.europarl.europa.eu/news/en/press-room/20240223IPR18095/meps-back-plans-for-an-eu-wide-digital-wallet)
* [EU Health Data Space must be individual-centric to benefit all stakeholders](https://mydata.org/2023/12/13/eu-health-data-space-must-be-individual-centric-to-benefit-all-stakeholders/)
* [EU Digital Identity Wallet](https://ec.europa.eu/digital-building-blocks/sites/display/EUDIGITALIDENTITYWALLET/EU+Digital+Identity+Wallet+Home)
* …

# \*\*\*\*\*\*\*\*\*\*\*\*

# Project Documentation

We are international 😊. We have supporters with a variety of backgrounds, therefore our documentation is in English.

## Project Team

![SSI Heatlh Team.png](https://s3.dribdat.cc/odch/a/374/KI99WMGPZ7R9FXPH0I408DOH/SSI_Heatlh_Team.png)

* [Peter Janes](https://www.linkedin.com/in/peterjanes/), Abdagon AG, Founder and CEO (peter.janes@abdagon.com); DIDAS Health Lead - Challenge Owner
* [Florian Bürgi](https://www.linkedin.com/in/florian-b%C3%BCrgi-7224b449/) \- wallet loader
* [Gian Derungs](https://www.linkedin.com/in/gian-valentin-derungs-482358176/) \- schemas\, proof request
* [Raphael Guye](https://www.linkedin.com/in/raphaelguye/) \- doctor's platform
* [Richard Lagrange](https://www.linkedin.com/in/richard-lagrange/) \- Azure environment
* [Bryan Raymonenq](https://www.linkedin.com/in/bryan-reymonenq/) \- patient
* [Lars Ruddigkeit](https://www.linkedin.com/in/drlr1/)

Please note that we are aiming to produce a short video about the activities of our challenge team. Let us know if you don't want to appear on images.

## Supporters

* [Roman Zoun](https://www.linkedin.com/in/roman-zoun/), Adnovum AG, Head Security Solutions Offerings; DIDAS Adoption Lead - Challenge Co-Owner
* [Daniel Hegedues](https://www.linkedin.com/in/daniel-hegedus-025916170/), Adnovum AG, Senior Software Engineer - VCMS Supporter, remote
* [Timothy Rabozzi](https://www.linkedin.com/in/rabozzi/), Adnovum AG, Innovation Developer - on-site
* [Jan Carlos Janke](https://www.linkedin.com/in/jan-carlos-janke/), HSLU, Business Development Manager; DIDAS Community Manager - on-site 14.03.2024
* [Michel Sahli](https://www.linkedin.com/in/michelsahli/), Federal Office of Justice, E-ID Innovation Fellow
* ...

## Schema Mapping from FHIR (subsets)

[Logical schema](https://github.com/Abdagon/hackathon-2024-ssi-health/blob/main/health-ssi-schema.md) (with Entity-Relationship-Diagram)

* [patient](http://www.hl7.org/fhir/patient.html)
* [insuranceProof](http://fhir.ch/ig/ch-core/StructureDefinition-ch-core-patient.html)
* [allergyIntolerance](http://www.hl7.org/fhir/allergyintolerance.html)
* [practitioner](http://www.hl7.org/fhir/practitioner.html)
* [observation](http://www.hl7.org/fhir/observation.html)
* [medicationRequest](http://www.hl7.org/fhir/medicationrequest.html)

## Technical Environment

* Verifiable Credential Management System (VCMS)
    * [Documentation](https://github.com/SSI-Solutions/vcms/tree/main)
    * API Definitions (Swagger Format)
        * [Connector](https://vcms-int.westeurope.cloudapp.azure.com:9080/swagger-ui/index.html)
        * [Issuer](https://vcms-int.westeurope.cloudapp.azure.com:9081/swagger-ui/index.html) (run /issue/credentials/definitions for credential Anoncred schemas)
        * [Verifier](https://vcms-int.westeurope.cloudapp.azure.com:9084/swagger-ui/index.html)
* [GitHub Repository](https://github.com/Abdagon/hackathon-2024-ssi-health) (initial data model)
* [GitHub Repository](https://github.com/needToRoll/govTechHack24-ssi-health) (code)
* [Google Drive](https://drive.google.com/drive/folders/1eYZ7r8O8wqiZ7xaN8JV_eoUPMVM466Va) (Viewer, Editor requires invitation with Google Account)

## Executing the Project

### Discussing Options

![Discussing Options.png](https://s3.dribdat.cc/odch/a/374/96TJ8YFT8P2EIGF0YAEH94S0/Discussing_Options.png)

### Desiging the Solution

![Design Solution.png](https://s3.dribdat.cc/odch/a/374/OWZOQ5RQYUZRZ5ADZ1A1Z6UM/Design_Solution.png)

### Defining the Schema

![Credential Schema.png](https://s3.dribdat.cc/odch/a/374/ECAYJ3DW98S7X42BIOUTQVL7/Credential_Schema.png)

[Gian Derungs](https://www.linkedin.com/in/gian-valentin-derungs-482358176/)

### Loading the Wallet

![Wallet Loader.png](https://s3.dribdat.cc/odch/a/374/7KJJ1R121I2SWPNH9CTHHA5I/Wallet_Loader.png)

[Florian Bürgi](https://www.linkedin.com/in/florian-b%C3%BCrgi-7224b449/)

### Building the Patient Wallet

![Patient Wallet.png](https://s3.dribdat.cc/odch/a/374/CR29PRMPR42ZB4XLV5OR3USF/Patient_Wallet.png)

[Bryan Raymonenq](https://www.linkedin.com/in/bryan-reymonenq/)

### Building the Doctor's Platform

![Doctors Platform.png](https://s3.dribdat.cc/odch/a/374/C1TNXQWHP2DDSBOS7V3PQE74/Doctors_Platform.png)

[Raphael Guye](https://www.linkedin.com/in/raphaelguye/)

### Integrating the Components

![Hacking Team.png](https://s3.dribdat.cc/odch/a/374/09QF9NY8R8MDX4OMSK25HQZL/Hacking_Team.png)

10 PM - still hard at work - and having fun

## The Result

Stay tuned - more to follow shortly!

## Final Pitch and Prize

Winning the award in the future oriented category - handed over by [Federal Chancellor Viktor Rossi](https://www.bk.admin.ch/bk/de/home/bk/bundeskanzler.html):
![Prize Stage.png](https://s3.dribdat.cc/odch/a/374/B9DJ6L4C76NYLC6FUOLRDZS3/Prize_Stage.png)

Our phantastic team on stage for the award ceremony.

![Prize Team.png](https://s3.dribdat.cc/odch/a/374/7K9JW08DXTN5JDDWFMHQK7ZJ/Prize_Team.png)

Our phantastic team - with [Federal Chancellor Viktor Rossi](https://www.bk.admin.ch/bk/de/home/bk/bundeskanzler.html) and [FOITT Director Dirk Lindemann](https://www.linkedin.com/in/dlindemann/).

## «Making of» Video

Showcasing team organization, work on the challenge and the final pitch with a live demonstration of the solution.

https://youtu.be/uNrMFE2wOyQ

## Positioning and Next steps

As correctly stated by jury member [Philippe Gillieron](https://www.linkedin.com/in/philippegillieron/), the challenge must be considered in the context of the current Swiss EPR initiative (EPD).

We anticipate a development of citizen oriented EHR information in three stages:

1. Document oriented («EPD 1.0») - current version, where information is mostly stored as reports in PDF-Format. A document oriented approach makes searches and automated processing alsmost impossible, which is particularly relevant with high volumes of documents.
2. Structured health information, server-based («EPD 2.0») - recognizing the limitations of document oriented information, there is wide agreement that clinical information must be available in structured and standardized formats to ensure semantic interoperability. Server-based technologies are readily available for such implementations.
3. Structured health information, wallet-based («EPD 3.0») - The very same standards can also be implemented based on SSI principles in the form of trustworthy «verifiable credentials» in digital wallets, which are part of the upcoming E-ID trust infrastructure.

There will certainly be extended transition periods and overlaps between the above stages, but the earlier we start prototyping, the sooner we can benefit from new possibilities.

The objective of our challenge was to demonstrate how a wallet-based healthcare use case can look like. We plan to further develop the prototype both on the use case and technology side. With this, we aim for further demonstrations to and feedback from the caregiver and citizens target groups.
