# porous materials AI gym

open data sets for machine learning pertaining to porous materials.

- MOF = metal-organic framework
- COF = covalent organic framework

<p align="center">
<img width="200px" src="nott300.png"/>
</p>

## crystal structures

### experimental

- MOFs: CoRE MOFs ([Paper](https://doi.org/10.1021/acs.jced.9b00835), [Database](https://zenodo.org/record/3677685)), CSD MOF Subset ([Paper](https://pubs.acs.org/doi/abs/10.1021/acs.chemmater.7b00441), [Database](https://sites.google.com/view/csdmofsubset/home)), CSD MOF Collection ([Paper](https://doi.org/10.1016/j.matt.2021.03.006), [Database](https://www.ccdc.cam.ac.uk/Community/csd-community/csd-mof-collection/))
- COFs: CURATED COFs ([Paper](https://pubs.acs.org/doi/10.1021/acscentsci.9b00619), [Database](https://github.com/danieleongari/CURATED-COFs)), CoRE COFs ([Paper](https://doi.org/10.1016/j.ces.2017.05.004), [Database](https://github.com/core-cof/CoRE-COF-Database))
- zeolites: IZA database ([Database](http://www.iza-structure.org/databases/))

### hypothetical

- MOFs: B&W ([Paper](https://www.nature.com/articles/s41586-019-1798-7), [Database](https://doi.org/10.24435/materialscloud:2018.0016/v3)), ToBaCCo ([Paper](https://pubs.acs.org/doi/abs/10.1021/acs.cgd.7b00848), [Database](https://mof.tech.northwestern.edu/databases), [Code](https://github.com/tobacco-mofs/tobacco_3.0)), hMOFs ([Paper](https://www.nature.com/articles/nchem.1192), [Database](https://mof.tech.northwestern.edu/databases)), Anderson et al. ([Paper](https://chemrxiv.org/articles/preprint/Deep_Learning_Combined_with_IAST_to_Screen_Thermodynamically_Feasible_MOFs_for_Adsorption-Based_Separation_of_Multiple_Binary_Mixtures/14122901/1), [Database](https://osf.io/7dgvy/)), MOF-5 analogues ([Paper](https://doi.org/10.1021/jp401920y), [Database](http://www.nanoporousmaterials.org/databases/)), PORMAKE ([Paper](https://doi.org/10.1021/acsami.1c02471), [Code](https://github.com/Sangwon91/PORMAKE))
- COFs: Mercado et al. ([Paper](https://doi.org/10.1021/acs.chemmater.8b01425), [Database](https://archive.materialscloud.org/record/2018.0003/v1)), Haranczyk's 3D COF database ([Paper](https://pubs.acs.org/doi/10.1021/jp507152j), [Database](http://www.nanoporousmaterials.org/databases/))

## labeled porous materials for supervised learning

| material class                       | target y                                             | features x provided?                 | Reference                                                                                                                    | size of data set |
| ------------------------------------ | ---------------------------------------------------- | ------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------- | ---------------- |
| MOFs (hypothetical)                  | CO2, N2 adsorption (sim)                             | yes                                  | [Paper](https://www.nature.com/articles/s41586-019-1798-7), [Database](https://doi.org/10.24435/materialscloud:2018.0016/v3) | ca. 325,000      |
| MOFs (experimental and hypothetical) | Band gaps, density of states, charge densities (sim) | yes                                  | [Paper](https://doi.org/10.1016/j.matt.2021.02.015), [Database](https://github.com/arosen93/QMOF)                            | ca. 18,000       |
| MOFs (experimental)                  | Color (exp)                                          | yes                                  | [Paper](https://doi.org/10.1039/D0SC05337F), [Database](https://doi.org/10.24435/materialscloud:cc-j6)                       | ?                |
| COFs (hypothetical)                  | CH4 deliverable capacity (sim)                       | yes, hand-crafted features provided. | [Paper](https://doi.org/10.1021/acs.chemmater.8b01425), [Database](https://archive.materialscloud.org/2018.0003/v3)          | ca. 70,000       |
| COFs (experimental)                  | CH4, H2, O2, Xe, Kr, H2S adsorption (sim)            | ?                                    | [Paper](https://doi.org/10.1021/acscentsci.0c00988)                                                                          | ca. 500          |
| MOFs (hypothetical)                  | H2 adsorption (sim)                                  | yes                   | [Paper](https://www.sciencedirect.com/science/article/pii/S2666389921001240#bib70) / [Database](https://datahub.hymarc.org/dataset/computational-prediction-of-hydrogen-storage-capacities-in-mofs)   | ca. 100K
| MOFs (experimental)                  | thermal stability, solvent removal stability         | yes (RAC & geometric features) | [Paper](https://www.nature.com/articles/s41597-022-01181-0)  / [Database](https://zenodo.org/record/5737968#.YjNo6lRlAuU) | ca. 2-3K (extracted from experimental lit)   

## labeled nodes for supervised learning

| material class                       | target y                               | Reference                                                                                                                                                                   | size of data set (# materials)            |
| ------------------------------------ | -------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| MOFs (experimental)                  | DDEC6 charges on atoms (sim)           | [Paper](https://doi.org/10.1021/acs.chemmater.5b03836), [Database](https://zenodo.org/record/3986573#.XzfKiJMzY8N)                                                          | ca. 3,000                                 |
| MOFs (experimental and hypothetical) | DDEC6/CM5/Bader charges on atoms (sim) | [Paper](https://doi.org/10.1016/j.matt.2021.02.015), [Database](https://github.com/arosen93/QMOF)                                                                           | ca. 18,000 (DDEC6/CM5), ca. 5,000 (Bader) |
| MOFs (experimental and hypothetical) | Effective bond orders on atoms (sim)   | [Paper](https://doi.org/10.1016/j.matt.2021.02.015), [Database](https://github.com/arosen93/QMOF)                                                                           | ca. 18,000                                |
| MOFs (experimental)                  | Formal oxidation states on atoms (exp) | [Paper](https://chemrxiv.org/articles/preprint/Using_Collective_Knowledge_to_Assign_Oxidation_States/11604129/1), [Database](https://doi.org/10.24435/materialscloud:dq-ey) | ca. 49,000                                         |

# other data sets, pertaining to materials, for machine learning

see `matminer` [here](https://hackingmaterials.lbl.gov/matminer/dataset_summary.html). pointed out by [Jack Evans](https://twitter.com/jackevansADL/status/1439730395570851841).

# construct your own crystal structures!
here is a list of open-source codes for building your own crystal structure models.

|   name of code  | link to code | link to associated paper |
| -- | -- | -- |
| `tobacco` | [link](https://github.com/tobacco-mofs/tobacco_3.0) | [link](https://pubs.acs.org/doi/abs/10.1021/acs.cgd.7b00848) |
| `pormake` | [link](https://github.com/Sangwon91/PORMAKE) | [link](https://pubs.acs.org/doi/full/10.1021/acsami.1c02471) |
| `ToBasCCo` | [link](https://github.com/peteboyd/tobascco) | [link](https://www.nature.com/articles/s41586-019-1798-7?proof=tNature) |
| `Zeo++` | [link](http://www.zeoplusplus.org/) | [link](https://pubs.acs.org/doi/abs/10.1021/cg500158c) |
| `stk` | [link](https://aip.scitation.org/doi/10.1063/5.0049708) | [link](https://github.com/lukasturcani/stk) |
| `PoreMatMod.jl` (only modifies) | [link](https://github.com/SimonEnsemble/PoreMatMod.jl) | [link](https://pubs.acs.org/doi/10.1021/acs.jcim.1c01219) |
| `pyCOFBuilder` | [link](https://github.com/lipelopesoliveira/pyCOFBuilder) | [link](https://arxiv.org/abs/2310.14822) |

