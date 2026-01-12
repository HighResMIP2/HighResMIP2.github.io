---
layout: default
title: CMIP7 Experiment
permalink: /experiments/experiment_cmip7/
---

We have developed an update to the HighResMIP1 experimental design towards CMIP7. The main differences are in the atmosphere-only simulations, and extending the coupled future simulations to 2100. The exact value for "present" in the following is undecided and will be influenced by CMIP7, likely around 2022.

### HighResMIP CMIP7 protocol
The HighResMIP2 protocol towards CMIP7 has been submitted, and the new output requirements for the Data Request will need further discussion.

### Tier 1a: Forced-atmosphere runs 1980-present
Experiment name: **highresSST-present**: Using ESA CCI forcing for SST and sea-ice (daily, 0.05 degree, updated through 2023 currently). 

### Tier 1b: Coupled control runs 1950-2050
Spin-up:  50 year spin-up from EN4 ocean climatology with constant 1950's forcing. Experiment name: **spinup-1950**  
Control:   100 years with 1950's forcing.        Experiment name: **control-1950**  

### Tier 2: Coupled historic and future runs 1950-2100.
Historic:  1950-present  with historic forcing.     Experiment name: **hist-1950**  
Future:    present-2100 with scenario forcing.      Experiment name: **highres-future-sspxxx**  

### Tier 3: Idealised experiments for CMIP-like metrics
Plus 4K experiment: Add 4K to SSTs used in highresSST-present. Experiment name: **highresSST-p4kuni**
Abrupt 4xCO2 experiment: Abrupt 4xCO2 forcing starting from the end of spinup-1950. Experiment name: **abrupt4xCO2-1950**

### Tier 4: Forced-atmosphere warming levels
Forced atmosphere simulations at different patterned warming levels, e.g. +2K, +4K, over 2003-2022. Plan to construct and use both warming and cooling trend patterns in Eastern Pacific. Experiment name: **highresSST-pxxkpat**

### Tier 5: One year experiment
A one year experiment (likely 2020 to link with DYAMOND2), to link with other communities.        Experiment name: **highres-yrxxxx**  
Associated +4K simulation. Experiment name: **highres-yrxxxx-p4kuni**

### Motivation of these five Tiers

Focus of HighResMIP is on the 1950-2100 period (Tier 2) for coupled simulations - extended from 2050 due to demand and feedback from HighResMIP1. This period includes significant past changes and the time horizon for the future is relevant for decision makers.

The division of the forced-atmosphere (AMIP-style) runs in Tier 1 and Tier 3 is to enable NWP centers to participate. It has been made shorter in order to use higher resolution SST/sea-ice forcings, and also to make it possible to use higher resolutions/produce more ensemble members. The "future climate" has been made explicitly idealised by using warming levels, either constant addition to SST (+4K to link to CMIP metrics), or patterned SST/reduced sea-ice at e.g. +2K, +3K.

Resolution: Atmosphere sub-50 km (ideally 10-25km); Ocean sub-0.25 degree (ideally eddy-rich)

Experiments are ideally repeated with standard resolution (but not enforced). Any lower resolution version would ideally link to CMIP DECK runs, but it is understood that higher resolution configurations take longer to develop, so older configurations are also encouraged.

HighResMIP philosophy: If tuning is necessary it should be well documented to ensure any improvements are due to process representation.

### Further proposed targeted experiments
Further sensitivity experiments are possible and await suggestions:

### HighResMIP2 CMIP7 simulation design

<a href="/assets/images/documents/highresmip_simulations_cmip7.png"> highresmip_simulations_cmip7 </a>

### HighResMIP2 schematic indicating uses of simulations

<a href="/assets/images/documents/highresmip2_schematic_forpaper.png"> highresmip_simulations_cmip7 </a>
