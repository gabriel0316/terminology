> **Für die deutsche Version bitte [hier](index.html) klicken.**

### Welcome to the new Austrian e-Health Terminology Browser!

The terminology server offers the stakeholders of the Austrian health care system the possibility to provide terminologies via the Internet and enables terminology research as well as terminology download in different formats. The goal is to enable IT systems that are in a data exchange relationship with each other to use the same terminologies at the same time. Code systems and value sets are made easily accessible together with the associated historical versions in standardized formats and uniform metadata.

### Technology basis

Technologically, the Austrian e-Health terminology system is based on TerminoloGit. See the [technical documentation](technical_documentation_en.html).

### FAQ

The most important questions and answers about the terminology server are summarized here.

#### Where can I find code lists and value sets that I have used so far?
Via [Table of Contents](https://termgit.elga.gv.at/toc.html) and [Artifact Summary](https://termgit.elga.gv.at/artifacts.html), respectively, the terminologies can be retrieved. For easier readability, only the postfixes (e.g. "_CS" or "_VS") have been removed. As soon as you click on a terminology, the details, such as whether it is a code system or value set, are displayed in the summary.

Table of Contents lists all terminologies alphabetically. Under the Artifact Summary, all terminologies are grouped by code systems or value sets.

An advanced search is still to be implemented.

#### What are the download formats? How do the new formats correspond to those of the old terminology server?

Currently, the following download formats are offered under the 'Download' tab of the respective terminology:

| *new* Terminologieserver | *old* Terminologieserver | Note |
| ----------- | ----------- | ----------- |
| FHIR R4 xml `.4.fhir.xml` | no correspondence       | |
| FHIR R4 json `.4.fhir.json`   | no correspondence        | |
| fsh v1 `.1.fsh`   | no correspondence        | |
| fsh v2 `.2.fsh`   | no correspondence        | |
| ClaML v2 `.2.claml.xml`   | ClaML        | |
| ClaML v3 `.3.claml.xml`   | no correspondence        | |
| propCSV v1 `.1.propcsv.csv`   | no correspondence        | |
| SVSextELGA v1 `.1.svsextelga.xml`   | SVS        | **Warning! DEPRECATED!**<br/>This format can technically not contain all the information<br/>that is available in the other formats.<br/>This format is only available for legacy purposes. |
| SVSextELGA v2 `.2.svsextelga.xml`   | SVS        | **Warning! DEPRECATED!**<br/>This format can technically not contain all the information<br/>that is available in the other formats.<br/>This format is only available for legacy purposes. <br/>However, all concept properties are available. |
| outdatedCSV v1 `.1.outdatedcsv.csv`   | CSV according to TermPub standard        | **Warning! DEPRECATED!**<br/>This format can technically not contain all the information<br/>that is available in the other formats.<br/>This format is only available for legacy purposes. |
| outdatedCSV v2 `.2.outdatedcsv.csv`   | CSV as it is <br/>supplied by TermPub <br/>(based on TermPub standard).        | **Warning! DEPRECATED!**<br/>This format can technically not contain all the information<br/>that is available in the other formats.<br/>This format is only available for legacy purposes. <br/>However, all concept properties are available. |

A more detailed description of each download format can be found [in the technical documentation](file_formats_en.html).

#### How do I know which terminology is the current one?

The terminologies that can be displayed and accessed via [Table of Contents](https://termgit.elga.gv.at/toc.html) or [Artifact Summary](https://termgit.elga.gv.at/artifacts.html) always represent the most recent versions.

Table of Contents lists all terminologies alphabetically. Under the Artifact Summary, all terminologies are grouped according to code systems or value sets.

#### Where can I find old versions?

With the new terminology server, all published versions can be called up for each terminology under the tab `Previous Versions`. When old versions are displayed, a warning is shown that this is an old version. This notice also includes a link to the current terminology version.

The old terminology server was operated until October 2022. If specific old versions of terminologies (prior to 2022) are sought, they can be requested from the CDA team [cda@elga.gv.at](mailto:cda@elga.gv.at).

#### How can I be notified of updates?

See [automatic import of terminologies](use_cases_en.html#automatic-import-of-terminologies) or [manual import of terminologies](use_cases_en.html#manual-import-of-terminologies).

#### How to suggest changes or report bugs?

Please, refer to the [support page](support_en.html).

### The ELGA & Austrian eHealth terminologies.

In ELGA and the Austrian eHealth systems, a large number of different terminologies with different structures are used from various international, national and local sources. TerminoloGit is used to bring these into as uniform a form as possible and make them visible here.

All terminologies and their changes can be accessed centrally on the terminology server and are also made known with update messages at https://confluence.elga.gv.at/display/SCCTERM. Checks for changed terminologies should be performed at least **weekly**.

All questions regarding ELGA- and Austrian e-Health-relevant terminologies that cannot be answered with this documentation can be reported to [cda@elga.gv.at](mailto:cda@elga.gv.at). Processing is coordinated centrally from this address.

For terminologies, a distinction is made between code systems and value sets.

#### Code systems

A code system is understood to be the collection of codes, their metadata and the metadata of the code system. Code systems can also be an ontology, table, or simple enumeration. [LOINC](https://loinc.org/), [SNOMED CT](https://www.snomed.org/), and [HL7® CodeSystems](https://www.hl7.org/fhir/codesystem-gender-identity.html) are examples of such code systems.

The updating of code systems and their timing or frequency is the responsibility of the creators and thus mostly beyond the control of ELGA. Code systems can only be corrected outside the responsibility of the creators if there is a technical problem.

A code system is uniquely identified not only by a unique name but also by an OID. The meaning of a code can only be deciphered together with the name/URI or OID of the code system.

A principle of terminology development is that codes must not be deleted, nor must the meaning of a code be changed [^1]. Such changes create an inconsistency in the use of older coded data with the current version of the code system. Typically, such "incompatible" version states of the code system are given different names/URI and OIDs to keep them apart (e.g., the annual versions of ICD-10). Not all code systems adhere to this requirement in practice. ELGA GmbH specifically highlights these updates, and we ask you to note the update messages at https://confluence.elga.gv.at/display/SCCTERM/ for this purpose. When adopting updates from such code systems, proceed with caution.

#### Value Set

Wherever a value selection is made by e.g. ELGA CDA implementation guides, a suitable Value Set is defined and specified with its unique name. ELGA Value Sets refer, with a few exceptions, to a specific "version" of one or more code systems, which can be identified by the unique name/URI of the code system. This makes the Value Sets independent of changes in the code systems. In addition, Value Sets can contain their own sequence and tree structure (hierarchy).

All Value Sets used in the implementation guides are published here at the Austrian Terminology Browser. It applies to all Austrian e-Health terminologies that the Value Sets are kept extensional, which means that the concepts are explicitly listed in the Value Set and are not dynamically linked with e.g. filters via the code system. Furthermore, the expansion of the ValueSet is always present.

How often Value Sets are changed depends on the respective application. Value Sets that are needed for "structural" elements (e.g. in the CDA header, XDS metadata) will rarely change. "Content" Value Sets (e.g. for drug lists, laboratory analyses, diagnosis codes) will have to change correspondingly frequently, here annual to weekly changes are to be expected. In exceptional cases, it is possible to specify when defining a value set that it must not be changed or versioned (ValueSet.immutable is set to true).

In the case of ELGA Value Sets that are subject to a regular maintenance and update cycle, extensions and changes can be made after technical review by the responsible content administrator (e.g. ELGA laboratory parameters, ASP list). In the case of other corrections to the content of ELGA Value Sets, the technical decision of the working group [^2] which developed the corresponding guideline within the framework of which the Value Set was defined may have to be obtained.

Contents of Value Sets may change, but the name and OID of a Value Set remain the same. For new versions, version number with release date (in ValueSet.version with e.g.: 2.3.1+20220618) and modification date (ValueSet.date) are specified. This allows to reconstruct the validity at a certain time.

Value Sets are valid until the date of a newer version of this Value Set is reached - then the newer version is valid. As long as no newer version exists, a Value Set remains valid (for exception "static" see also chapter [Value Set Binding](#value-set-binding)). If codes are not allowed to be used any more, a new version of the Value Set is created, in which the codes not to be used any more are set to inactive=true. These codes are kept in the ValueSet only for historical reasons. The new version is valid from the upload unless the status of the Value Set has been set to draft and the date is in the future.

##### Value Set Binding

For ELGA and the Austrian eHealth systems, a DYNAMIC binding to Value Sets applies in principle. This means that the version of a Value Set currently published on the terminology server must always be used. (The explicit setting of the corresponding keyword 'DYNAMIC' is therefore not required in the guidelines).

Value Sets can also be STATICALLY bound to a code element. This is indicated by specifying the Value Set with name/URI, OID, version and date (ValueSet.date) and the keyword `STATIC`.

#### Versioning

The following versioning is implemented only after the end of parallel operation. As long as the old terminology server is maintained, it must be ensured that the versioning on the old and new terminology servers match.

The following versioning scheme applies to the versioning of terminologies such as code systems or value sets:

    MAJOR.MINOR.PATCH+YYYMMDD

For individual terminologies such as CodeSystems or ValueSets the following applies:

* `MAJOR` is incremented if, for example.
   * the intent or definition of the full terminology changes;
* `MINOR` is incremented if, e.g.
	* a concept is added;
	* a concept is deprecated/retired;
	* the DisplayName of a concept is changed;
   * the metadata of a concept changes and thus the meaning of the concept is extended/reduced;
   * the structure/grouping (e.g. for the ValueSet) changes;
* `PATCH` is increased, if e.g.
    * spelling errors or typos in the metadata (not DisplayName or code) of an existing concept are corrected.
* `YYYMMDD` corresponds to the date from which the terminology applies.

##### Status transition diagram for concepts

The following status transition diagram applies to all concepts in code systems or value sets:

[![status_life_cycle_for_concepts](https://gitlab.com/elga-gmbh/termgit/-/raw/main/input/images/status_life_cycle_for_concepts.png){: style="width: 100%"}](https://gitlab.com/elga-gmbh/termgit/-/raw/main/input/images/status_life_cycle_for_concepts.png)

Here, the mapping between LOINC® and FHIR® R4 is as follows:

LOINC↓ FHIR Code System → |
|  | **Active**&ensp;  | **Deprecated**&ensp; | **Retired**&ensp; | **Experimental**&ensp; |
|---|---|---|---|---|
| **Active** | X |  |  |  |
| **Discouraged** |  | X |  |  |
| **Deprecated** |  |  | X |  |
| **Trial** |  |  |  | X |

The mapping between SNOMED CT® and FHIR® R4 is as follows:

SNOMED CT↓ FHIR code system → | | | | | |
|  | **Active**&ensp; | **Deprecated**&ensp; | **Retired**&ensp; | **Experimental**&ensp; |
|---|---|---|---|---|
| **Active** | X |  |  |  |
| **Inactive** |  | X |  |  |


### GitLab project overview

The content of the [Austrian e-Health Terminology Browser](https://termgit.elga.gv.at/) is based on the following two GitLab projects:

| Project Name | Description | Repository URL | GitLab Project ID | GitLab Pages URL |
| --- | --- | --- | --- | --- |
| TerminoloGit | [https://gitlab.com/elga-gmbh/termgit](https://gitlab.com/elga-gmbh/termgit) | Repository for published, up-to-date terminologies (download formats).<br/><br/>*Note:* The contents of the last successful pipeline of any Git branch of this repository are displayed under the specified GitLab Pages URL. | 33179072 | [https://elga-gmbh.gitlab.io/termgit](https://elga-gmbh.gitlab.io/termgit) |
| TerminoloGit HTML | [https://gitlab.com/elga-gmbh/termgit-html](https://gitlab.com/elga-gmbh/termgit-html) | Repository for the static HTML pages created by the HL7® FHIR® IG Publisher based on the `main` branch of [https://gitlab.com/elga-gmbh/termgit](https://gitlab.com/elga-gmbh/termgit). | 33179017 | **[https://termgit.elga.gv.at](https://termgit.elga.gv.at)** |
### Roles

The Terminology Server is primarily a system for providing code lists and value sets; it is not intended to provide real-time access for processing by information systems. The Terminology Server is not currently used as an online resource (for checking individual values), but as a source for new terminologies to be stored locally.
The terminology server is used by the following user groups:

| user group | task | GitLab.com role | description |
| --- | --- | --- | ---|
| Terminology Consumer | reading access | none, not required | As a terminology consumer, no self-registration is required for viewing and exporting terminologies or checking for new versions. |
| Terminology Manager | Terminology Maintenance | Developer | The creation or update of terminologies is done by the Terminology Manager. It is not possible to assign a responsible user to each terminology. |
| Terminology Administrator | Release and Publication | Maintainer | Before terminologies become publicly available, they are released by a terminology administrator. |

### Publication process for terminologies created by external publishers

The following process is defined for the publication of terminologies created by ELGA-external terminology manager for the Austrian e-Health Terminology Server.

#### Requirements

- Basic knowledge of Git or GitLab is assumed to be known.
- The desired terminology is not subject to external licensing requirements and already has its own OID. If there is no OID for the terminology yet, it can be requested via the [OID platform](https://www.gesundheit.gv.at/OID_Frontend/application.htm?section=5).
- The release process and procedure explained below are familiar.

#### Release process

1. status "draft": Only certain users are allowed to create, modify or import terminologies. Each terminology has a terminology administrator. Terminology administrators can modify and technically release all terminologies. All newly created or newly imported terminologies or terminology versions have the status draft/draft and are only visible in their own Git branch.
2. status "for release" (draft with merge request): The terminology owner releases the content of the terminology version, and the terminology thereby assumes this new status (still only visible in its own Git branch, which has now issued a merge request).
3. status "released" (active): The created or modified terminologies are also available to terminology consumers after a release by a terminology administrator (have been moved to the master/main Git branch).
4. status "invalid" (retired): These terminologies may not be used (anymore). This can have two triggers:
   1. the created draft was rejected by the terminology administrator.
   2. the assigned terminology owner or a terminology administrator withdraws the version and manually sets it to invalid.

[![Release Process](https://gitlab.com/elga-gmbh/termgit/-/raw/main/input/images/Freigabeprozess.png "Release Process"){: style="width: 100%"}](https://gitlab.com/elga-gmbh/termgit/-/raw/main/input/images/Freigabeprozess.png)

#### Procedure

1. Contact ELGA GmbH via e-mail address [cda@elga.gv.at](mailto:cda@elga.gv.at) with **[completed application form](files/Applicationform_external_terminology_developer_de.pdf)** (currently available in German only):
   1. Name of the terminology
   2. OID of the terminology
   3. Code system/value set
      1. In case of a value set: disclosure of the associated code system(s)
   4. Description of the terminology (DE and EN)
   5. Person and organization responsible for the terminology
      1. Name (organization)
      2. E-mail address (organization)
      3. Name (responsible person)
      4. E-mail address (responsible person)
   6. GitLab.com user who is to contribute the terminology to the GitLab project [TerminoloGit](https://gitlab.com/elga-gmbh/termgit). The nomination of more than one GitLab.com user is possible.
2. The completed form will be checked technically and legally by ELGA GmbH.
3. After successful verification, "Developer" rights will be granted to the GitLab users named by the applicant in the GitLab project [TerminoloGit](https://gitlab.com/elga-gmbh/termgit). This allows the user to create branches, but not to merge into the default branch of the project without approval by a user with "Maintainer" rights.
4. For the initial creation of the import file, **import templates** for **[code system](files/CodeSystem-cs-import-template.1.propcsv.xlsx)** or **[value set](files/ValueSet-vs-import-template.1.propcsv.xlsx)** are provided in the form of CSV files. The required attributes are described in the section [Proprietary CSV](file_formats_en.html#proprietary-csv-propcsv---csv-and-xlsx).
   1. Uploading to the GitLab project can be done via different ways (e.g. GitLab WebIDE or software like Sourcetree). For questions and support, the external terminology manager can contact the TerminoloGit team ([cda@elga.gv.at](mailto:cda@elga.gv.at)).
   2. Thematically related terminologies should be edited together in one branch to maintain clarity.
   3. Commits must comply with Git governance: [https://cbea.ms/git-commit/](https://cbea.ms/git-commit/)
   4. Terminologies from external terminology manager are collected under a separate category named after the organization name.
5. After completion of the terminology, a merge request is created so that the branch can be merged into the default branch.
   1. The technical review is performed by the ELGA GmbH.
   2. If the technical requirements are met, the branch is merged to the default branch.
6. After the pipelines have been successfully run, a check is made to ensure that the desired terminologies have been published correctly and completely.
7. Finally, the terminology manager is informed about the publication and an update of the [Semantic Competence Center changelist](https://confluence.elga.gv.at/display/SCCTERM/Terminologien+-+Changelist+2022) is published.

### References

[^1]:Concept Permanence, described in "Cimino's Desiderata" (Desiderata for Controlled Medical Vocabularies in the TwentyFirst Century; 1998; [http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3415631/](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3415631/))
[^2]:  A "CDA Advisory Board" that makes decisions by circular resolution (qui tacet consentit). The decisions made can be made public by mail distribution list.
