
_WIP_

# Curation summary

The Universal Chalcidoidea Database is curated by a distributed team of chalcidologists. This document lays out the general scope of what is being curated (Scope), and the means of that curation (Tasks).  Specifics are found in the Manual. 

## Nomenclature

### Scope

Our intent is to catalog chalcid nomenclature, as goverened by the [ICZN](https://code.iczn.org/), comprehensively.  In brief this means that, sensus the ICZN, all availble, unavailble, valid, and invalid names for chalcid wasps are targets for cataloging. For the purposes of our curation unavailable names are those for which the author _intended_ to be treated by the ICZN, but failed for reasons based on the rules therein.  For example, "jewel wasp" was never intended to be goverened, so while techinical the name is unavaible, it doesn't fall in this category for the purposes of curation. 

A list of common names is not being curated.

Secondarily, we are discussing the role of non-governed names, particularly those for molecular vouchers, which are increasing and relatively prominent in the chalcid literature. These names are linked to concepts, and individual specimens. Recording them as OTU labels, then linking those OTUs to the nomenclature requires some discussion of what the link between the OTU label (`name` field in TaxonWorks) and the nomenclature name (`taxon_name` in TaxonWorks) _means_. [How do we structure this discussion?]

### Tasks

Curation in this area focuses on:
* The addition of Sources via the "New source hub" task
* The addition of taxon names, their authors, status (synonym), and original combination via the "New taxon name" task
* The addition of taxonomic history via the "New combination" task [and things such as new synonymies, revised status, etc.]
* The validation and review of nomenclature via the "Browse nomenclature" task

## Annotated bibliography

### Scope

Noyes used over 100 different topics (e.g. "Biology", "Distribution") as tags in conjunction with citations on taxon names. These annotations are now included on both Taxon Names, when they involve nomenclatural actions, and OTUs, when they concern biology.

Moving forward curators will focus on a smaller subset of these, each of which will be provided a definition, and if possible, the concept linked to a corresponding ontology term:

* TODO, provide list of terms to be curated. 
* TODO, point to Controlled Vocabulary Terms manager task instead of default new CVT term

### Pertinent tasks and interfaces

* The Controlled Vocabulary Term Data card for a list of Topics
* The radial annotator for Taxon Names and OTUs
* The "Browse annotations" task to visualize per topic
* The "Browse taxa" page to visual topics per citation
* The "Content editor" task to apply Topics per text content

## Biological associations

### Scope

At the time of transfer there were 115,213 biological associations assigned between OTUs. Our intent is to continue capturing all biological associations between parasitoids and hosts. Additional non-parasitoid related relationships, for example `found_on` will not be comprehensively gathered but may be added by curators if they wish.

Noyes used 6 biological relationships, "Plant associate", "Associate", "Parasitoid", "Parasitoid host", "Plant host", "Primary host". Because some of the properties in the labels of these relationships can be inferred by the name assigned to the OTU (plant, animal, and, because of the chaining of relationship "Primary"), we can simplify the relationships used down to a shorter list. Relationships can be assigned from either "side" in the interface facilitating this shorter list.

* parasitoid / host - e.g. given A parasitoid / host B then A is a parasitoid and B is a host
* associate / associate - e.g. given A associate B then A is an associate of B, and B is an associate of A

Noyes also added extensive annotations about the parasitoid type. In TaxonWorks these were migrated as internal data attributes. Some of these data could be integrated into specific relationships if we choose to do so, basically expanding the relationships greatly to include the particular type on either side. A simple ontology/hierarchy may facilitate this assignment. [what are some examples of these parasitoid types?  Not clear what this is]  

### Pertinent tasks and interfaces

* The Biological Associations Data card
* The Biological Relationships Data card
* The "OTU radial" to assign biological relationships
* The "Browse taxa" page to list biological relationships
* The "Data attributes" page to list annotations on associations
* The "Annotation radial" to add relationships type values to the biological associations

## Geographic distribution

### Scope

At the time of transfer there were 105,049 geographic distribution assertions. Our intent is to capture all distributions down to 3rd level geographic subdivisions (e.g. counties in the USA). While not required, and with no intent to be comprehensive, curators may also curate individual specimens, particularly types, assigning georeferences to their associated collecting events.

### Pertinent tasks and interfaces

* The Asserted Distributions Data card
* The "Browse asserted distributions" Task
* The "New asserted distribution" Task
* The "New asserted distribution from map" Task
* The "Asserted distributions - basic endemism" Task
* The "OTU radial" to assign and site distributions.

## Type material

### Scope

Noyes did not explicitly create specimen records, but rather added type data to name records. These data from the UCD were attached to Taxon names (nomenclature) as data attributes in TaxonWork. Moving forward we will capture all primary-type records as specimen records. Non-primary type information can also be recorded as specimen records but is not required.

There is a strong desire to begin to comprehensively catalog images of the primary types.  It seems likely that this will become a "required" component for UCD@TW.

### Pertinent tasks and interfaces

* The "Comprehensive digitization" task for type speicmens
* The simpler "New type specimen task" available through the new taxon name task
