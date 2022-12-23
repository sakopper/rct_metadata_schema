# RCT Metadata schema crosswalk

## Version 0.9.0

*Note: The current version is 0.9.0 because it is a preliminary and tentative mapping, without recent feedback from stakeholders of the other schematas we map to. We will continue to version up as we receive that feedback and make any edits.*

## Content:

This folder currently consists of "Crosswalk_RCT_Metadata.xlsx." Its purpose is to provide information on mapping the RCT metadata schema to other social science metadata schematas. 

It currently contains mappings to the following schematas:

- The World Bank Microdata Catalog (API and guide for data archivists)
- Dataverse (The citation, geographic, and social science/humanities metadata blocks)
- Clinicaltrials.org
- YARD/ISPS
- AEA Trial Registry
- DDI Codebook 2.5

### Columns:

The crosswalk currently has 8 groups of columns:

- **A-D**: Contain a copy of the metadata schema as presented in Appendices A and B in this repository.
- **E-G**: Contain information on the development of the field, including whether it is a new creation, and if not, the schema we drew the definition from, the original definition, and any changes we mafe to the field.
- **H-K**: Information on mapping to the World Bank Microdata Catalog. The first two columns are the placement of symmetric fields in the API and guide for data archivists, respectively, the third is for notes, and the last is a description of the mapping.
- **L-N**: Mapping to the Dataverse. The structure of this and each of the following groups of columns follows the above.
- **O-R**: Mapping to clinicaltrials.org
- **S-U**: Mapping to YARD/ISPS
- **V-x**: Mapping to the AEA Trial Registry
- **Y-AB**: Mapping to DDI Codebook 2.5. Column AA contains notes from a DDI expert that were obtained earlier in the schema creation process.

### Types of mapping:

The "Type of map" column in each of the last six column groupings above contains one of the following values, which attempt to describe how information could be shared between a catalog based on the RCT metadata schema and catalogs based on other schemata.

- **One-to-one:** The fields are equivalent; information can easily be transferred between one field and the other with minimal difficulty/loss of information.
- **One-to-one but cardinality different:** The fields are equivalent other than a difference in cardinality. For version 0.9.0 only repeatable (and not optionality) was taken into account, so any fields that are currently marked with this value have a different number of potential repititions in the two schemata.
- **One-to-one but encoding schemes different:** The fields are equivalent other than the method with which they are filled in. An example is a mapping from a free text field to one with a controlled vocabulary.
- **RCT more granular:** The fields contain broadly the same information, but the RCT metadata schema asks for more specific information or a subset of the information asked for in the field in the mapped schema.
- **RCT less granular:** The fields contain broadly the same information, but the other metadata schema asks for more specific information or a subset of the information asked for in the field in the RCT metadata schema.
- **Some information transfer possible:** The fields are different, but their scopes are similar enough that some information transfer would be possible.
- **Unsure if information transfer possible:** A mapping appears unlikely, but more information is needed before marking it as not mappable.
- **Mapping currently unlikely:** The field in the RCT metadata schema is different enough from all fields in the other schema that a mapping does not seem likely at this time.    