---
description: EPIC Public Beta v2.0.0
---

# Methodology

EPIC compares a base case against a set of carbon reduction measures. User-defined sets of carbon reduction measures can be saved as scenarios and compared.

### [Base Case](../users-guide/base-case/)

In EPIC, the base case is defined as the case resulting from a set of conservative assumptions representing a project in which no efforts have been made to reduce carbon emissions, constructed solely as a means of comparison for evaluating carbon reduction measures. The base case in EPIC is always new construction. In many municipalities, code requirements (e.g. California’s Title 24 energy codes) will mean that EPIC’s base case is not equivalent to a code baseline. The base case overrides on the Project Base Case tab can adjust some of EPIC’s internal variables; any changes to these will be applied across all scenarios.

EPIC assesses the efficacy of the carbon reduction measures in relative terms, as a reduction in the total carbon emissions from a base case. EPIC’s base case is not equivalent to a baseline in wbLCA, which must be functionally equivalent to all other wbLCA options. This is not possible within EPIC as salient carbon reduction measures, such as building a smaller building, may result in a building that is not functionally equivalent to the base case.

### [Carbon Reduction Measures](../users-guide/carbon-reduction-measures/)

Each carbon reduction measure (CRM) modifies one or more of the parameters in EPIC's data model. In almost all cases, modifying these parameters will reduce the base case carbon emissions. In some cases, however, emissions may increase (e.g. changing a wood frame structure to steel).

The measures are divided into three categories (embodied, operational, and landscape), but many measures have effects across categories: Some CRMs affect individual variables (specifying low-carbon concrete changes the carbon intensity of a single input), some affect multiple model components by changing a single variable (reducing the building’s area will lower both its operational and embodied emissions), and other change multiple variables across many model components (adding a photovoltaic array incurs embodied emissions but lower operational emissions).

### [Scenarios](../users-guide/carbon-reduction-measures/scenarios.md)

A user-defined set of carbon reduction measures is called a scenario. By saving and comparing scenarios, a user can compare the overall reductions that different sets of CRMs can accomplish, identify the contributions of individual CRMs, and evaluate tradeoffs between CRMs.
