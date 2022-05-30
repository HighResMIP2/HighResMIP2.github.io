---
layout: default
title: CMIP6 Experiment
permalink: /experiments/experiment_cmip6/
---

We developed an experimental design for CMIP6, and are developing modifications to this for future experiments and towards CMIP7.

### HighResMIP CMIP6 protocol
The HighResMIP protocol is described in detail in [Haarsma et al 2016](http://www.geosci-model-dev-discuss.net/gmd-2016-66/). It was one of the official MIP projects for WCRP's CMIP6 HighResMIP.  
The HighResMIP output requirements are described in the [Data Request](https://earthsystemcog.org/projects/wip/CMIP6DataRequest%20CMIP6).  
Below is a short outline of the protocol

#### Tier 1: Forced-atmosphere  runs 1950-2014
Experiment name: **highresSST-present**: Using HadISST2.2.0.0 1/4 degree SST and sea-ice forcing dataset - see [sst-and-sea-ice-forcing](../sst_seaice_forcing/)

#### Tier 2: Coupled runs 1950-2050
Control:   100 years with 1950's forcing.        Experiment name: **control-1950**  
Historic:  1950-2014  with historic forcing.     Experiment name: **hist-1950**  
Future:    2015-2050 with SSP585 forcing.        Experiment name: **highres-future**  
Spin-up:  50 year spin-up from EN4 ocean climatology with constant 1950's forcing. Experiment name: **spinup-1950**  

#### Tier 3: Forced-atmosphere 2015-2050 (2100)
2015-2050 with SSP585 forcing (and future SST/sea-ice fields).  Experiment name: **highresSST-future**

#### Motivation of these three Tiers

Focus of HighResMIP is on the 1950-2050 period (Tier 2). This period includes significant past changes and the time horizon for the future is relevant for decision makers.

The division of the forced-atmosphere (AMIP-style) runs in Tier 1 and Tier 3 is to enable NWP centers to participate. It also includes the possibility for end of the century simulations.

Resolution: Atmosphere 20-50 km; Ocean ~0.25 degree

Experiments are repeated with standard resolution. This version is also the entry for DECK runs.

HighResMIP philosophy: No or minimal additional tuning for high resolution version. If tuning is necessary it should be well documented.

#### Further proposed targeted experiments
We never had enough groups willing to do additional idealised experiments, but these may be ideas to take forwards into the updated HighResMIP:

Leaf area index (LAI) experiment highresSST-LAI  
Smoothed SST highresSST-smoothed  
CFMIP style experiments highresSST-p4K; highresSST-4co2  
Abrupt 4XCO2 highres-4co2  
