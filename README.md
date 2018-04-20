# UFSCOMP

The **Unified Forecast System Community Portal (UFSCOMP)** is an entry point for community members interested in obtaining NOAA’s Unified Forecast System (UFS) for their own interests and experimentation. The UFS utilizes a set of forecast system software components to build a suite of targeted, predictive applications spanning spatial and temporal scales. It will include multiple Earth system model components (e.g. atmosphere, ocean, sea ice) and software to support a complete forecast workflow including data pre-processing, data assimilation, model coupling, ensemble and probabilistic processing, post-processing, and experiment management. *At this time, UFSCOMP includes only a small subset of the UFS.*

This portal aims to reduce barriers to sharing code between research and operational groups. It simplifies UFS access by providing the needed linkages to model component and infrastructure code located in distributed repositories. These linkages change based on the particular UFS application (e.g. Finite Volume Cubed-Sphere Dynamical Core - Global Forecast System or FV3-GFS) and the particular version of that application requested. This makes it difficult to assemble a working application without prior knowledge of the constituent components. To address this, UFSCOMP provides configurations of UFS components that are versioned, documented, tested, and have clearly identified supported platforms/machines and dependencies. Additionally, initial conditions data files are downloaded automatically from the CESM public input data repository.

## Supported Applications

- [CMEPS v0.1](https://github.com/ESCOMP/UFSCOMP/wiki/Milestone:-CMEPS-0.1) - Modular Ocean Model version 6 (MOM6) coupled with the Community Mediator for Earth Prediction Systems (CMEPS)
