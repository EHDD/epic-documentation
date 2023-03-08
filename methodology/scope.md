# Goal and Scope

## Goal

EPIC is a design tool that integrates assessments of embodied, operational, and sequestered carbon in a data model to support low-carbon design at the earliest stages of a project.

EPIC is designed for use during site and feasibility studies, requests for proposals, pre-design, and in other early-phase activities where quantitative support is needed for low-carbon design decisions and a whole-building life cycle assessment is not practicable. EPIC is not comprehensive: the tool uses a data model to assess the carbon emissions associated with, and the effects of carbon reduction measures on, some components of a project for some stages of a project’s life cycle. EPIC's scope is designed to maximize a designer's ability to assess low-carbon design strategies in early project phases within the limitations of currently available data. EPIC is a work in progress; future development will respond to user feedback, incorporate improved data, and refine the tool's methodology.

## Scope

### Time Horizon

EPIC can accommodate time horizons of 30 or 60 years. Currently, the web application can only accommodate a 30 year time horizon. For analysis on a 60 year time horizon, [use our API](../access-epic-via-api.md).&#x20;

### Life Cycle Stages

EPIC integrates data from life cycle stages (sometimes called "life cycle modules") A1-A5, B2-B6, and C2-C4. These correspond to the impacts of the materials used in the project, emissions from  construction, their replacement over time, and the project’s operational energy use. When biogenic carbon is counted, some end-of-life impacts (from modules C3-C4) are assessed during the product phase (see appendix [Biogenic Carbon](../backmatter/biogenic-carbon.md)).

<figure><img src="../.gitbook/assets/EPIC Life Cycle Stages.png" alt=""><figcaption><p>Highlighted life cycle stages are included in EPIC.</p></figcaption></figure>

### Embodied Carbon Scope

EPIC includes an assessment of embodied carbon from the following sources:

* Building structure and foundation
* Construction activities
* Cladding, glazing, and roofing and their replacement over time
* Interior fit-out and its replacement over time
* MEP systems and their replacement over time
* PV arrays and their replacement over time
* Regular landscape maintenance, assessed annually

### Operational Carbon Scope

EPIC considers operational emissions from the following sources:

* Emissions from the combustion of methane gas in the building
* Upstream leakage of methane gas as a proportion of methane gas combusted in the building
* Upstream emissions from the generation of electricity delivered to the site

### Stored Carbon Scope

EPIC includes an estimate of carbon storage in timber structural systems and site landscaping. Carbon storage in planting is calculated over the time horizon then annualized. Carbon storage in building structure is assigned to the first year of the project. EPIC's method for calculating carbon storage in timber structural systems is detailed in the appendix on [biogenic carbon](../backmatter/biogenic-carbon.md).

### Refining EPIC's Scope

In EPIC, you can add or remove some life cycle modules and building components from the scope of a project. When comparing results between EPIC models, between EPIC and wbLCA, or between any estimates of carbon emissions, _the scopes of each result must be identical._&#x20;

When EPIC's scope is defined for a given project, that same definition of scope will be used in each of the project's scenarios. More information on how to define the scope fo analysis within EPIC is in the user's guide \[\[HERE]].
