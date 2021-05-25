# porous materials AI gym
open data sets for machine learning pertaining to porous materials.
* MOF = metal-organic framework
* COF = covalent organic framework

<p align="center">
<img width="200px" src="nott300.png"/>
</p>

## crystal structures

#### experimental
* MOFs [link](https://doi.org/10.1021/acs.jced.9b00835)
* COFs [link](https://pubs.acs.org/doi/abs/10.1021/acscentsci.9b00619), [link](https://www.sciencedirect.com/science/article/pii/S000925091730310X)
* zeolites [link](http://www.iza-structure.org/databases/)

#### hypothetical
* COFs [link](https://doi.org/10.1021/acs.chemmater.8b01425)
* MOFs [link](https://www.nature.com/articles/s41586-019-1798-7)


## labeled porous materials for supervised learning

| material class | target y | features x provided? | DOI | size of data set|
| ----------- | ----------- | ----------- | ----------- | ----------- | 
| COFs (hypothetical) | CH4 deliverable capacity | yes, hand-crafted features provided. | 10.1021/acs.chemmater.8b01425 | ca. 70,000 |
| MOFs (hypothetical) | CO2, N2 adsorption | ? | 10.1038/s41586-019-1798-7 | ca. 325,000 |
| COFs (experimental) | CH4, H2, O2, Xe, Kr, H2S adsorption | ? | 10.1021/acscentsci.0c00988 | ca. 500 |

## labeled nodes for supervised learning
| material class | target y | DOI | size of data set|
| ----------- | ----------- | ----------- | ----------- | 
| MOFs (experimental) | point charges on atoms | 10.1021/acs.chemmater.5b03836 | 2,000 |
| MOFs | point charges on atoms | 10.1016/j.matt.2021.02.015 | 14,000 |
