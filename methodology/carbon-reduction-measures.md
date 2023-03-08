# Model Structure

### EPIC calculates "whole carbon" emissions

EPIC integrates embodied, operational, and landscape carbon emission assessment. Calculation procedures for each are detailed in the follow parts of this guide:

* [Calculating Embodied Carbon](calculations.md)
* [Calculating Operational Carbon](calculations-1.md)
* [Calculating Stored and Avoided Carbon](calculations-2.md)

### EPIC is built on time series data

The time value of carbon is important, so EPIC uses time series data to analyze carbon emissions across a building's life. For each year in the analysis period (defined by the project's [time horizon](scope.md#time-horizon)), EPIC estimates all emissions occurring in that year. For a thirty year reference period from 2025 to 2034, EPIC's summary emissions estimates are calculated as:

$$total\ emissions = \sum_{n=2025}^{2034}[emissions_{embo,n}+emissions_{oper,n}+emissions_{land,n}]$$

**In the first year**, the following emissions are always calculated:

* Embodied emissions in construction materials (life cycle stages A1-A3)
* Construction site emissions (life cycle stages A4-A5)
* Storage of biogenic carbon in timber structural components (life cycle stage D)

**In the each year**, the following emissions are always calculated:

* Operational carbon emissions from onsite fossil fuel use (life cycle stages B6)
* Operational carbon emissions from onsite electricity use (life cycle stages B6)
* Emissions from landscape maintenance, when applicable  (life cycle stages B2)

**In only some years,** the following emissions are always calculated:

* Replacement and refurbishment of hardscape (life cycle stages B3-B5)
* Replacement and refurbishment of the building envelope (life cycle stages B3-B5)
* Replacement and refurbishment of interior fit-out (life cycle stages B3-B5)
* Replacement and refurbishment of MEP and PV systems (life cycle stages B3-B5)

### EPIC is customizable and extensible

EPIC's model is built as a series of modules, each connected to the others and tasked with a specific set of calculations.  These modules are added or expanded in response to the requests of users.&#x20;

Many parts of the EPIC model (in v2.0.0 and beyond) can be customized or overriden by the user. This allows for the addition of project-specific data where it is available while maintaining the EPIC model for calculating all other parts of the project's carbon footprint. More information about the set of customizations available in the open access web app is available \[HERE].&#x20;















&#x20;&#x20;
