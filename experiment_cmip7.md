---
layout: default
title: CMIP7 Experiment
permalink: /experiments/experiment_cmip7/
---

We are developing an update to the HighResMIPv1 experimental design towards CMIP7. The main differences are in the atmosphere-only simulations, and extending the coupled future simulations to 2100. The exact value for "present" in the following is undecided and will be influenced by CMIP7, likely around 2022/23.

### HighResMIP CMIP7 protocol
The HighResMIPv2 protocol towards CMIP7 is being developed, as well as the new output requirements for the Data Request. The details are still under discussion, with an aim for a full proposal by end-2023. Below is a short outline of the current proposal.

### Tier 1a: Forced-atmosphere runs 1980-present
Experiment name: **highresSST-present**: Using ESA CCI forcing for SST and sea-ice (daily, 0.05 degree, updated to 2022 currently). 

### Tier 1b: Coupled control runs 1950-2050
Spin-up:  50 year spin-up from EN4 ocean climatology with constant 1950's forcing. Experiment name: **spinup-1950**  
Control:   100 years with 1950's forcing.        Experiment name: **control-1950**  

### Tier 2: Coupled historic runs 1950-present.
Historic:  1950-present  with historic forcing.     Experiment name: **hist-1950**  

### Tier 3a: Forced-atmosphere warming levels
Forced atmosphere simulations at different warming levels, including +4K experiment.  Experiment name: **highresSST-warming-levels**

### Tier 3b: Coupled future present-2100
Future:    present-2100 with scenario forcing.        Experiment name: **highres-future-sspxxx**  

### Tier 4: One year experiment
A one year experiment (exact year TBD), to link with other communities.        Experiment name: **highres-one-year-xxxx**  

### Motivation of these four Tiers

Focus of HighResMIP is on the 1950-2100 period (Tier 2) for coupled simulations - extended from 2050 due to demand and feedback from HighResMIPv1. This period includes significant past changes and the time horizon for the future is relevant for decision makers.

The division of the forced-atmosphere (AMIP-style) runs in Tier 1 and Tier 3 is to enable NWP centers to participate. It has been made shorter in order to use higher resolution SST/sea-ice forcings, and also to make it possible to use higher resolutions/produce more ensemble members. The "future climate" has been made explicitly idealised by using warming levels, either constant addition to SST (+4K to link to CMIP metrics), or patterned SST/reduced sea-ice at e.g. +2K, +3K.

Resolution: Atmosphere sub-50 km (ideally 10-25km); Ocean sub-0.25 degree (ideally eddy-rich)

Experiments are ideally repeated with standard resolution (but not enforced). Any lower resolution version would ideally link to CMIP DECK runs, but it is understood that higher resolution configurations take longer to develop, so older configurations are also encouraged.

HighResMIP philosophy: If tuning is necessary it should be well documented to ensure any improvements are due to process representation.

### Further proposed targeted experiments
Further sensitivity experiments are possible and await suggestions:

 
