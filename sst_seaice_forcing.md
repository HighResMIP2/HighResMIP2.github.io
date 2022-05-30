---
layout: default
title: SSTSeaiceForcing
permalink: /experiments/sst_seaice_forcing/
---

<h3> SST and sea-ice forcing used for CMIP6 HighResMIP</h3>
Many studies have shown that gradients in SST associated with fronts and ocean eddies can have significant influence on the atmosphere via changes in air-sea fluxes. Similarly, there is evidence that daily variability rather than monthly smoothed forcing can influence model simulations . Since the high resolution simulations will approach 25km, this means there is a requirement for a daily, 1⁄4 degree dataset for a period longer than satellite-based datasets are able to provide.

Hence, we will use a new dataset based on HadISST2.2.0.0 (Kennedy et al., The Met Office Hadley Centre Sea Ice and Sea-Surface Temperature data set, version 2.2.0.0, Technical Note, in prep) which has these properties for both SST and sea-ice concentration for the period 1950-2014 – in addition, it provides an ensemble of historic realizations which can potentially be used to produce multiple ensemble members.

The dataset is HadISST2.2.0.0, and is now available on the input4MIPs web site [Inputs4MIPs](https://esgf-node.llnl.gov/search/input4mips) - use HighResMIP or HadISST search criteria. The dataset is derived from a quarter degree daily version of HadISST2.1.1.0 from pentad data for the period 1948-2014. While the full documentation is still being developed, this is a brief summary of the method (courtesy of Nick Rayner and John Kennedy at the Met Office Hadley Centre):

HadISST2.2.0.0 SST and sea-ice forcing on 1/4 degree daily grid:
The ability to produce 0.25 degree fields of actual SST comes from our use of a satellite-era climatology. The analysis of residuals from that climatology (aka anomalies) which we do on a 5-day timescale is performed on a 1 degree grid. On that spatial and temporal scale, that analysis is perfectly achievable with the data available and is done both for pre-satellite data and satellite-era data alike. Information on covariances between anomalies in different locations gained from the satellite (and in situ) data enables the analysis to be done at the same resolution throughout. The ensemble captures the uncertainty in this process and its spread is wider prior to the satellite era.

Links to the documentation will appear here when it is available.
[Link to the dataset in CMIP6 inputs4MIPs](http://doi.org/10.22033/ESGF/input4MIPs.1221)

HighResMIP future forcing
The SST and sea-ice concentration forcing for the future atmosphere-only simulation (highresSST-future) is now available at inputs4MIPs:
[Link to the future forcing dataset in CMIP6 inputs4MIPs](https://esgf-node.llnl.gov/search/input4mips/?institution_id=MOHC&amp;target_mip_list=HighResMIP&amp;query=version:20190308)

The methodology used to create this forcing datasets is described at
[Methodology for constructing future forcing](https://github.com/PRIMAVERA-H2020/HighResMIP-futureSSTSeaice)