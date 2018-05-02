# UFSCOMP

*This portal has been set up for exploratory purposes and does not contain any validated Unified Forecast System (UFS) codes at this time. The coupled codes it contains are early prototypes that are not official National Weather Service products. External model components that are referenced in the coupled codes contained here, such as MOM6, follow their own terms of use.*

The **Unified Forecast System Community Portal (UFSCOMP)** is an entry point for community members interested in obtaining and running NOAA’s Unified Forecast System (UFS) for their own interests and experimentation. The UFS utilizes a set of forecast system software components to build a suite of targeted, predictive applications spanning spatial and temporal scales. It will include multiple Earth system model components (e.g. atmosphere, ocean, sea ice) and software to support a complete forecast workflow including data pre-processing, data assimilation, model coupling, ensemble and probabilistic processing, post-processing, and experiment management. *At this time, UFSCOMP is a prototype that includes only a small subset of the full UFS functionality.*

This portal aims to reduce barriers to sharing code between research and operational groups. It simplifies UFS access by providing the needed linkages to model component and infrastructure code located in distributed repositories. These linkages change based on the particular UFS application and the particular version of that application requested. This makes it difficult to assemble a working application without prior knowledge of the constituent components. To address this, UFSCOMP provides configurations of UFS components that are versioned, documented, tested, and have clearly identified supported platforms/machines and dependencies. Initial condition data files are downloaded automatically from a public input data repository, and a [portable model workflow](https://github.com/ESMCI/cime) makes running the system easier.

## Supported Applications

The UFSCOMP repository supports multiple applications (or "apps") where an app is an assembly of external components, each referenced by a repository URL and a branch/tag. An app, therefore, is a convenient way to represent known configurations of components and can be easily shared. The top level app repository is *lightweight* because all information about the external components is stored in a single configuration file (`Externals.cfg`).

*Each app is stored on a separate branch in the UFSCOMP repository.* Each app branch is prefixed with `app_`. The current app branches:
- **app_mom6-cmeps** - Modular Ocean Model version 6 (MOM6) coupled with the Community Mediator for Earth Prediction Systems (CMEPS)
- **app_cesm-cmeps** - Community Earth System Model (CESM) components coupled with the CMEPS Mediator

## Milestones

- [CMEPS v0.1](https://github.com/ESCOMP/UFSCOMP/wiki/Milestone:-CMEPS-0.1) - Initial validation of Modular Ocean Model version 6 (MOM6) coupled with the Community Mediator for Earth Prediction Systems (CMEPS)
