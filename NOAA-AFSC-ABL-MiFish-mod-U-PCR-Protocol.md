---
# MIOP terms
methodology_category: Omics Analysis
project: NOAA AFSC ABL Environmental DNA Lab Protocols
purpose: PCR [OBI:0000415]
analyses: PCR [OBI:0000415]
broad_scale_environmental_context: marine biome [ENVO:00000447], freshwater biome [ENVO:00000873]
local_environmental_context: marine biome [ENVO:00000447], freshwater biome [ENVO:00000873]
environmental_medium: sea water [ENVO:00002149], fresh water [ENVO:00002011]
target: 12S mitochondrial ribosomal RNA  [NCIT:C128263], MT-RNR1 Gene [NCIT:C128260]
creator: Kimberly Ledger, Diana Baetscher
skills_required: sterile technique, pipetting skills, standard molecular technique
time_required: 150 minutes
personnel_required: 1
language: en
issued: 2025-06-04
audience: scientists
publisher: NOAA Alaska Fisheries Science Center Auke Bay Laboratories Genetics Program
hasVersion: 1
license: CC0 1.0 Universal
maturity level: mature

# FAIRe terms
pcr_0_1: 1
thermocycler: Applied Biosystems GeneAmp PCR System 9700
amplificationReactionVolume: 12
assay_name: mifish-u-12s
assay_validation: not provided
targetTaxonomicAssay: 12S rRNA gene sequencing targeting the V5-V6 region using primers MiFish-U-F_mod and MiFish-U-R
targetTaxonomicScope: fishes
target_gene: 12S rRNA
target_subfragment: V5-V6
ampliconSize: 163/185
pcr_primer_forward: GCCGGTAAAACTCGTGCCAGC
pcr_primer_reverse: CATAGTGGGGTATCTAATCCCAGTTTG
pcr_primer_name_forward: MiFish_U_F_mod
pcr_primer_name_reverse: MiFish_U_R
pcr_primer_reference_forward: 10.1098/rsos.150088 | 10.1016/j.scitotenv.2020.142096
pcr_primer_reference_reverse: 10.1098/rsos.150088
pcr_primer_vol_forward: 0.12
pcr_primer_vol_reverse: 0.12
pcr_primer_conc_forward: 10
pcr_primer_conc_reverse: 10
probeReporter: not applicable
probeQuencher: not applicable
probe_seq: not applicable
probe_ref: not applicable
probe_conc: not applicable
commercial_mm: Qiagen Multiplex PCR Plus
custom_mm: PCR reactions were run in triplicate in 12 uL reaction volumes, with 2.0 uL of DNA, 6 uL of Qiagen Multiplex PCR Plus, 3.76 uL of water, and 0.12 uL of each primer (10 uM)
pcr_dna_vol: 2.0
pcr_rep: 3
nucl_acid_amp: 
pcr_cond: initial denaturation:95_5;denaturation:95_0.5;annealing:60_0.5;elongation:72_0.5;final elongation:68_10;35
annealingTemp: 60
pcr_cycles: 35
pcr_analysis_software: not applicable
pcr_method_additional: not applicable
---

# Protocol Template - PCR

## PROTOCOL INFORMATION

### Minimum Information about an Omics Protocol (MIOP)

- MIOP terms are listed in the YAML frontmatter of this page.
- See [MIOP_definition.md](https://github.com/BeBOP-OBON/0_protocol_collection_template/blob/main/MIOP_definition.md) for list and definitions.

### Making eDNA FAIR (FAIRe)

- FAIRe terms are listed in the YAML frontmatter of this page.
- See <https://fair-edna.github.io/download.html> for the FAIRe checklist and more information.
- See <https://fair-edna.github.io/guidelines.html#missing-values> for guidelines on missing values that can be used for missing FAIRe or MIOP terms.

### Authors

| PREPARED BY | AFFILIATION | ORCID | DATE |
| ------------- | ------------- | ------------- | ------------- |
| Kimberly Ledger | Genetics Program, Auke Bay Laboratories, Alaska Fisheries Science Center, NOAA | https://orcid.org/0000-0002-5552-5598 | 2025-06-04 |
| Diana Baetscher | Genetics Program, Auke Bay Laboratories, Alaska Fisheries Science Center, NOAA | Content Cell | 2025-06-04 |

### Related Protocols

| PROTOCOL NAME | LINK         | VERSION      | RELEASE DATE | INTERNAL/EXTERNAL |
| ------------- | ------------ | ------------ | ------------ | ----------------- |
| NOAA-AFSC-ABL-DNA-Extraction-Protocol  | TBD | Content Cell | yyyy-mm-dd   | Internal  |
| NOAA-AFSC-ABL-Barcode-PCR-Protocol  | TBD | Content Cell | yyyy-mm-dd   | Internal  |

### Protocol Revision Record

| VERSION | RELEASE DATE | DESCRIPTION OF REVISIONS |
| ------------- | ------------- | ------------- |
| 1.0.0 | 2025-06-04 | Initial release |

- Version numbers start at 1.0.0 when the protocol is first completed and will increase when changes that impact the outcome of the procedure are made (patches: 1.0.1; minor changes: 1.1.0; major changes: 2.0.0).
- Release date is the date when a given protocol version was finalised.
- Description of revisions includes a brief description of what was changed relative to the previous version.

### Acronyms and Abbreviations

| ACRONYM / ABBREVIATION | DEFINITION |
| ------------- | ------------- |
| AFSC | Alaska Fisheries Science Center  |
| NOAA | National Oceanic and Atmospheric Administration|
| eDNA | environmental DNA  |
| PCR | polymerase chain reaction |
| NTC | no template control | 
| DI water | deionized water | 
| IDT| Integrated DNA Technologies

### Glossary

| SPECIALISED TERM | DEFINITION |
| ------------- | ------------- |
| Extraction blank  | Extraction negative control. Typically nuclease-free water or empty filter run through the DNA extraction process to control for contamination in the DNA extraction step. |
| Field blank  | Sampling negative control. Typically distilled or reverse osmosis water run through a filter like an seawater eDNA sample to control for contamination in the field sampling step. |
| No template control | PCR negative control. Typically nuclease-free water loaded in place of a sample on a PCR to control for contamination in the PCR step. |
| Positive control  | PCR positive control. Typically a synthetic DNA strand, non-indigenous DNA extract, or intentionally designed mock community loaded in place of a sample on a PCR to control for contamination and index hopping in the PCR step. |

## BACKGROUND

### Summary

This protocol describes steps for performing PCR for the 12S mitochondrial ribosomal RNA gene in vertebrates using eDNA. The primers (forward: MiFish-U-F_mod, reverse: MiFish-U-R) were first presented in Sales et al. 2019 (forward) and Miya et al. 2015 (reverse). The MiFish-U-F_mod primer used in this protocol has 1 basepair substition from the MiFish-U-F primer used in Miya et al. 2015, but is otherwise identical. The target amplicon size is 163 - 185 base pairs.

This primer set targets vertebrates organisms (e.g., fishes, marine mammals, birds). Important note, this primer also amplifies non-target organisms including microbes and single-celled phytoplankton (e.g., proteobacteria and diatoms).

The protocol presented here is intended as the first PCR of a two-step PCR next generation sequencing library preparation using Illumina Nextera Unique Dual Indices. Use NOAA-AFSC-ABL-Barcode-PCR-Protocol (in progress) to perform the second PCR step in which unique library-specific barcodes are attached to each round 1 PCR product. 

### Method Description and Rationale

This protocol was chosen because it has been tested and deployed at scale by the NOAA AFSC Genetics Program. While not identical, it closely aligns with partner research lab protocols at NOAA NMFS and NOAA PMEL OME. 

### Spatial Coverage and Environment(s) of Relevance

This protocol can be used to amplify the 12S marker gene region of any eDNA sample.

## PERSONNEL REQUIRED

One person with molecular biology experience.

### Safety

This protocol does not involve any hazardous chemicals, although standard precautions including wearing PPE should be taken to avoid skin and eye exposure to chemical reagents.

### Training Requirements

Molecular biology training (including, at a minimum, sterile technique, pipetting small volumes, and programming and running PCR thermocyclers) is required to conduct this protocol.

### Time Needed to Execute the Procedure

** PCR preparation and running the PCR protocol for a single 96-well plate takes 2.5 hours (150 minutes), of which XX mins is the thermocycler run time. Additional plates can be run simultaneously without greatly increasing the time required.

## EQUIPMENT

| DESCRIPTION | PRODUCT NAME AND MODEL | MANUFACTURER | QUANTITY | REMARK |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| **Durable equipment** |
| PCR workstation | Content Cell | Content Cell | Content Cell | Content Cell |
| Pipetter: 1-10 μl|Pipet-Lite LTS Pipette L-10XLS+ |Rainin|1|Can be substituted with any accurate pipettor|
| Pipetter: 20 - 200 μl	|Pipet-Lite LTS Pipette L-200XLS+ |Rainin|	1|Can be substituted with any accurate pipettor|
| Pipetter: 100-1000 μl	|Pipet-Lite LTS Pipette L-1000XLS+ |Rainin|1|Can be substituted with any accurate pipettor|
| 8-channel Pipetter: 1-10 μL| Pipet-Lite Multi Pipette L8-10XLS+ |Rainin| 1|Can be substituted with any accurate pipettor. Not required but reduces protocol time.|
| Vortex | Vortex Genie 2 | Scientific Industries | 1 | Can be substituted with generic|
| Plate centrifuge | Centrifuge 5430 | Eppendorf | 1| Can be substituted with generic|
| Mini-centrifuge | myFuge  | Benchmark | 1 | Can be substituted with generic, but needs to fit 1.5-2.0 mL tubes | 
| 1.5 or 2 mL tube cool rack | CoolRack M6 | Thermo Scientific  | 1 | Can be subsituted with generic |
| 2 mL tube rack | Microcentrifuge tube rack | unknown | 1 | Can be substituted with generic | 
| 96-well PCR plate cool rack | PCR-Cooler 0.2mL | Eppendorf | 1 | Can be substituted with generic|
| 96-well PCR plate rack | PCR tube rack for 96-well plates | unknown | 1 | Can be substituted with generic |
| Thermocycler | GeneAmp PCR System 9700 | Applied Biosystems | 1 | Can be substituted with generic |
| E-Gel Device| E-Gel Power Snap Electrophoresis Device | Invitrogen | 1 | Can be substituted with agarose gel electrophoresis system|
| **Consumable equipment** |
| 1000 μL filter pipette tips | Pipette Tips TR LTS 1000uL F | Rainin | 2 | Can be subsituted with generic - must be sterile, filtered, and match pipetter |
| 200 μL filter pipette tips  | Pipette Tips TR LTS 200uL F | Rainin| 3 | Can be subsituted with generic - must be sterile, filtered, and match pipetter|
| 10 μL filter pipette tips  | Pipette Tips TR LTS 20uL F | Rainin | 104 | Can be subsituted with generic - must be sterile, filtered, and match pipetter |
| 96-well PCR plate | Template semi-skirted 96-well PCR plate, 0.2 ML | USA Scientific | 1 | Can be substituted with generic |
| 8-well strip tube w/ caps | 0.2 mL 8-tube strips with caps | Bio-Rad | 1 | optional, Can be substituted with generic |
| foil plate seals | VWR Adhesive PCR Foil Seals | VWR | 1 | Can be substituted with generic |
| microcentrifuge tubes | GeneMate 1.7 uL microcentrifuge tube | VWR | 1 | Can be substituted with generic |
| disposable gloves | Comfort Nitril Gloves | Fisherbrand | 2 | Can be substituted with generic |
| E-Gel | E-Gel EX Agarose Gel | Invitrogen | 1 | Can be substituted with agarose gel |
| **Chemicals** |
| 2X PCR Master Mix | Qiagen Multiplex PCR Plus | Qiagen | 624 uL per plate | Store at -20C long-term, or in refrigerator for up to one week. |
| Forward Primer | Custom oligo| IDT | 12.5 uL per plate | Store at -20C long-term, or in refrigerator for up to one week.  |
| Reverse Primer | Custom oligo | IDT | 12.5 uL per plate | Store at -20C long-term, or in refrigerator for up to one week. |
| Nuclease-Free Water  | Ultrapure DNase/RNase-free distilled water | ThermoFisher Scientific | 1 mL | Can be substituted with generic |
| Positive control| Lake Sturgeon genomic DNA | N/A | 2 μl per plate |Store at -20°C |
| 70% EtOH | Molecular grade ethanol| Generic | 40 mL | |
| 10% bleach| Hypochlorite bleach |Clorox| 40 mL | Remake every ~5 days as bleach decomposes quickly at 10% concentration |

## STANDARD OPERATING PROCEDURE

### Protocol

#### Preparation

1. While wearing clean, disposable gloves, sterilize workspaces and durable equipment, including pipettes within the PCR workstation with 10% bleach. Then wipe down all surfaces and equipment with 70% EtOH.
2. Run the UV light in the PCR workstation for at least 10 minutes before starting work.
3. Label all PCR plates both on the side of the plate and on the top of the foil (in the plate margins). Recommended labeling scheme includes plate name, primer, date of PCR and personnel initials.

#### PCR

**Primer Sequences without Adapters**(not used in this protocol): PCR primer sequences
(**target sequence bolded**)

| PCR Primer Name | Direction | Sequence (5’ -> 3’)|
| ----- | ----- | ----- |
|MiFish-U-F_mod | Forward |**GCCGGTAAAACTCGTGCCAGC** |
|MiFish-U-R | Reverse | **CATAGTGGGGTATCTAATCCCAGTTTG** |

**Primer Sequences Used**: PCR primer sequences with Illumina Adapters
(Adapter sequence + **target sequence bolded**)
| PCR Primer Name | Direction | Sequence (5’ -> 3’)|
| ----- | ----- | ----- |
|MiFish-U-F-mod_wAdapter | Forward  | CGACAGGTTCAGAGTTCTACAGTCCGACGATC**GCCGGTAAAACTCGTGCCAGC** |
|MiFish-U-R-wAdapter |Reverse | GTGACTGGAGTTCAGACGTGTGCTCTTCCGATCT**CATAGTGGGGTATCTAATCCCAGTTTG** |

**Reaction Mixture**: PCR reagents, volumes, initial and final concentrations

| Reagent |Volume (μL) per plate| Volume (μL) per reaction | Intial concentration| Final concentration|
| ----- | ----- | ----- |----- |----- |
| Qiagen Multiplex PCR Plus |624 | 6.0 |100% |50% |
| Forward Primer | 12.5 | 0.12 |10 μM |0.1 μM |
| Reverse Primer | 12.5 | 0.12 |10 μM | 0.1 μM |
| Nuclease-Free Water |391| 3.76 | N/A|N/A |
| Template DNA|N/A| 2 | N/A | N/A |
| **Total**|**1040.0**| **12.0** | **N/A** |**N/A**|

This table breaks down the mixture per plate and per reaction. When running full plates (96-wells), each reagent volume was multipled by 104 (96+8 extra sample volumes to account for pipetting error) when preparing the final master mix.

**PCR Cycling Program**: 

| PCR step | Temperature | Duration | Repetition |
| ----- | ----- | ----- | ----- |
|Initial denaturation|	95°C	|5min|	1X
|**Normal Cycling**||||
|Denaturation|	95°C|	30s|	35X|
|Annealing|	60°C|	30s	|35X|
|Extension 	|72°C	|30s	|35X|
|Final extension	|68°C	| 10min	|1X|
|Hold	|4°C	|∞	|1X|

**Step-by-Step Instructions:**

*Note: PCR set-up should be carried out in a separate pre-PCR space that is distinct from where the post-PCR space where thermocyclers are located and all post-PCR processing is performed. No equipment, consumables, or reagents should be shared between pre- and post-PCR spaces with a unidirectional flow of sample processing.*

1. While wearing clean, disposable gloves, set out PCR master mix, primers, template DNA and positive control to thaw if frozen.
2. Briefly vortex (just a few pulses is sufficient) and spin down thawed PCR master mix, primers, positive control, and nuclease free water. Thawed reagents should be stored in a cooling block or fridge when not in use.
3. Pool reagents to make final master mix, as denoted in the above reaction mixture table. If primers are not at designated working concentration, make a dilution from the stock concentration first. 
4. Aliquot 10 μL of final master mix into each well of the PCR plate. If setting up a full 96-well plate, it is more efficient aliquot 130 μL of final master mix per well into a 8-well strip tube. Then use a multichannel pipet to transfer 10 μL of final master mix into 96-well plate. The plate should sit in a cold block to ensure the reagents remain at a low temperature.
5. Add 2 μL DNA template to each well, but reserve two wells for the positive control and a no template control (NTC). 
6. To one well each, add 2 μL of the positive control and 2 μL of nuclease-free water for the NTC.
7. Seal the PCR plate with foil and double check plate is labeled with plate name, primer, date of PCR and personnel initials. 
8. Briefly vortex (just a few pulses is sufficient) and spin down the plate, and then place in thermocycler.
9. Run PCR cycling program.

### Quality Control

1. Plates should be removed from the thermocycler after the run completes and stored at 4°C until run on a gel. Storing the PCR product at -20˚C is ideal for 1-6 month term storage.
2. Run gel visualization using E-Gel System confirm successful PCR and correct target size fragment. 

#### E-Gel Protocol
1. Insert pre-cast agarose gel into E-Gel device. 
2. Load 18 uL of DI water to every well (regardless of whether or not sample or ladder will be added). 
3. Add 2 uL of DNA ladder or PCR product into the wells (total volume per well is 20 uL). Note: You may reuse E-Gels and do not need to load a sample to every well in a single run. 
4. Select appropriate program and run gel for 10 minutes. Visualize using built-in light system. 

#### Positive Control

A positive control is used in every PCR run to verify success of the PCR reaction. In place of template DNA, 2 μL of positive control is used. One well per plate is alotted for the positive control. The positive control used for MiFish 12S is Lake Sturgeon (*Acipenser fulvescens*). Lake sturgeon is a North American freshwater fish that does not occur in study regions of the AFSC Genetics Program.

#### Negative Control

The inclusion of a negative control for PCR is to confirm the absence of contamination during the process. Nuclease-free water is used as a no template control (NTC) when setting up each PCR plate. One well per plate is alloted to a NTC. NTCs should be run in addition to both field blanks and extraction blanks.

## REFERENCES

1. Miya M., Sato Y., Fukunaga T., Sado T., Poulsen J. Y., Sato K., Minamoto T., Yamamoto S., Yamanaka H., Araki H., Kondoh M. and Iwasaki W. 2015MiFish, a set of universal PCR primers for metabarcoding environmental DNA from fishes: detection of more than 230 subtropical marine speciesR. Soc. Open Sci.2150088150088
http://doi.org/10.1098/rsos.150088
2. Sales NG, Wangensteen OS, Carvalho DC, Mariani S. Influence of preservation methods, sample medium and sampling time on eDNA recovery in a neotropical river. Environmental DNA. 2020; 00: 119–130. https://doi.org/10.1002/edn3.14
