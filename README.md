# JUMP-MOA
`JUMP-MOA` is list of compounds with diverse MOAs that fit on a single 384-well plate, with 4 replicates per compound. 
There are 90 compounds from 47 distinct MOA classes. The recommended concentration for these compounds is `3 uM`. 
This resource was created through the [JUMP-Cell Painting Consortium](https://jump-cellpainting.broadinstitute.org/).

The MOA annotations were obtained from https://clue.io/repurposing.

The company Specs has assembled the compounds for purchase; for info contact tamara.baptist@specs.net

## Files

[`JUMP-MOA_compound_metadata.tsv`](JUMP-MOA_compound_metadata.tsv)

| Column | Description |
| :----- | :---------- |
| broad_sample | Compound ID in Broad Institute's compound management database |
| InChIKey | [International Chemical Identifier](https://en.wikipedia.org/wiki/International_Chemical_Identifier) |
| pert_iname | Compound name |
| pubchem_cid	 | PubChem ID e.g. [`72716071`](https://pubchem.ncbi.nlm.nih.gov/compound/72716071) |
| moa | Mechanism-of-action annotation, derived from [Broad Drug Repurposing Hub](https://clue.io/repurposing) and curated [here](https://github.com/broadinstitute/lincs-cell-painting/blob/master/metadata/moa/repurposing_info_external_moa_map_resolved.tsv) |
| smiles | Simplified molecular-input line-entry system ([SMILES](https://en.wikipedia.org/wiki/Simplified_molecular-input_line-entry_system)) string |

[`JUMP-MOA_compound_platemap.tsv`](JUMP-MOA_compound_metadata.tsv)

| Column | Description |
| :----- | :---------- |
| well_position | Well position |
| broad_sample | Compound ID in Broad Institute's compound management database |
| solvent | Solvent (always DMSO) |

[`JUMP-MOA_compound_platemap_with_metadata.csv`](JUMP-MOA_compound_platemap_with_metadata.csv)

A csv with the combined information from the tsv's.

| Column | Description |
| :----- | :---------- |
| well_position | Well position |
| broad_sample | Compound ID in Broad Institute's compound management database |
| solvent | Solvent (always DMSO) |
| InChIKey | [International Chemical Identifier](https://en.wikipedia.org/wiki/International_Chemical_Identifier) |
| pert_iname | Compound name |
| pubchem_cid	 | PubChem ID e.g. [`72716071`](https://pubchem.ncbi.nlm.nih.gov/compound/72716071) |
| moa | Mechanism-of-action annotation, derived from [Broad Drug Repurposing Hub](https://clue.io/repurposing) and curated [here](https://github.com/broadinstitute/lincs-cell-painting/blob/master/metadata/moa/repurposing_info_external_moa_map_resolved.tsv) |
| smiles | Simplified molecular-input line-entry system ([SMILES](https://en.wikipedia.org/wiki/Simplified_molecular-input_line-entry_system)) string |

## Plate layout

![Plate layout](layout.png)

## De-identified compounds

Eight of these compounds have been de-identified; they have `broad_sample` values of `Compound1`, `Compound2`, ..., `Compound8`.
If you are recreating this plate, we recommend replacing these de-identified compounds with their (non-de-identified) counterparts i.e. the other compound in the set with the same MOA:

|moa                         |replace_with      |original  |
|:---------------------------|:-----------------|:---------|
|HMGCR inhibitor             |delta-Tocotrienol |Compound1 |
|kinesin inhibitor           |ispinesib         |Compound2 |
|BCL inhibitor               |ABT-737           |Compound3 |
|PARP inhibitor              |veliparib         |Compound4 |
|IGF-1 inhibitor             |NVP-AEW541        |Compound5 |
|tricyclic antidepressant    |dosulepin         |Compound6 |
|FGFR inhibitor              |BLU9931           |Compound7 |
|phosphodiesterase inhibitor |quazinone         |Compound8 |

## Broad internal notes

- Originally called CPJUMP-Stain1
- 90 compounds x 4 replicates
- Compound Request Number: CR-11516 - placed by Shantanu Singh - $2,950
- 3 milliMolar 10 uL total volume (5 uL dead volume)

