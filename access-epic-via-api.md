# Access EPIC via API

## Why use our API?

In addition to the open access version of EPIC available, the data model behind EPIC is accessible as an API. By directly integration of EPIC into their own platforms and workflows, our API has allowed our partners to:

* Analyze "look-ahead" scenarios for the construction or acquisition of large portfolios of buildings.
* Perform sensitivity testing of carbon reduction measures.
* Stress-test planning and policy decisions at the municipal, regional, or national scale.

API integration has also allowed organizations to extend EPIC to meet their specific needs:

* Supplement the EPIC model with building-specific data or organization-specific carbon reduction measures.
* Integrate EPIC into their existing ESG and carbon accounting platforms.
* Deploy a custom versions of EPIC to an organization's internal servers.

API access can be tailored to meet your organization's specific needs. If you are interested in learning more, [please contact our team](mailto:epic@ehdd.com?API).  &#x20;

## Overview of EPIC API <a href="#overview" id="overview"></a>

EPIC is a stateless API for calculating whole carbon footprints from buildings. EPIC has the ability to calculate embodied, operational, and landscape emissions at various levels of resolution. A description of EPIC's methodology for calculating carbon emissions is available in our [public-facing documentation](https://epic-documentation.gitbook.io/epic/) and additional information about our methods is available [upon request](mailto:epic@ehdd.com?subject=Methods) .EPIC's API is [RESTful](http://en.wikipedia.org/wiki/Representational\_State\_Transfer), has predictable URLs, accepts [JSON-encoded](http://www.json.org/) request bodies, returns [JSON-encoded](http://www.json.org/) responses, and uses standard HTTP response codes, authentication, and verbs.

### Data Dictionary <a href="#data-dictionary" id="data-dictionary"></a>

A full data dictionary for the 100+ parameters in EPIC is available to our partners. To learn more or preview the data structure, [please reach out](mailto:epic@ehdd.com?subject=API).

### Minimum Parameters <a href="#minimum-parameters" id="minimum-parameters"></a>

At each of its three endpoints, EPIC can calculate the emissions from a building from a small set of parameters. The seven minimum parameters are:

* `project name` : The name of the project.
* `year_completion` : The year in which work on the project is completed.
* `zipcode` : The postal code for the building's location.
* `primary_structural_system` : The description of the building's structural system.
* `primary_use` : The use type of the building.
* `above_floor_sqf` : The average area per floor for all above ground floors.
* `above_floors` : The number of floors above ground.



### Expanded API Calls <a href="#expanded-api-calls" id="expanded-api-calls"></a>

Only seven parameters are necessary to calculate a preliminary estimate with EPIC, but almost 100 additional parameters are available in the API to tune that estimate to better describe your specific case.

