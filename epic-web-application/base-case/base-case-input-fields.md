# Base Case Input Fields

### Project Information

**Project name**

Select a name for your project. This name will appear on graphics generated by EPIC and will be the name of the project on the EPIC website.

**Project Location**

The United States ZIP Code in which the project is located.

**Projected year of completion**

The year that construction is completed and building operation begins. This is the year to which construction emissions are attributed and the EPIC model begins calculating operational carbon emissions.

### Building Structure

**Primary structural system**

The base case structural system selected from the choices below:

<details>

<summary>Structural Systems included in EPIC</summary>

* _Composite_ s_teel frame_. A structural system comprised of steel columns, beams, and girders connected with rigid or pin joints. Floors are steel decking with a concrete topping slab.&#x20;

<!---->

* _Reinforced concrete_. A structural system comprised of columns, beams, and slabs of concrete reinforced with steel that provides tensile strength.

<!---->

* _Hybrid concrete/steel (high-rise)_. A structural system that combines rigid steel frames with concrete columns, beams, and slabs. These hybrid structures are more materially intensive and may be used when there are significant seismic loads, in high-rise buildings, or for programs with very high live or environmental loads.

<!---->

* _Wood frame_. A structural system comprised of dimensional lumber, plywood sheathing, and reinforced concrete cores and podiums.

<!---->

* _Comprehensive mass timber_. A structural system comprised of massive beams, panels, and columns, often assembled by aggregating many smaller timber elements. This approach assumes that timber elements are aggressively substituted for other structural materials.

</details>

### Building Use

**Primary Use**

The use category from the list below most reflective of the project’s main use. This is used to determine the building's energy use and its structural requirements.&#x20;

**Secondary Use**

If the primary use comprises less than 100% of the program, a secondary program may be selected for the remainder. This program will affect the EUI (resulting in a ‘blended EUI’) but will not affect the estimate of the building’s structural system.

<details>

<summary>Use Categories included in EPIC</summary>

* Aquarium&#x20;
* Convention Center&#x20;
* Distribution Center&#x20;
* Dormitory&#x20;
* Fitness Center&#x20;
* Hospital&#x20;
* Hotel&#x20;
* K-12 School&#x20;
* Laboratory&#x20;
* Library&#x20;
* Medical Clinic&#x20;
* Multifamily Housing&#x20;
* Museum Office&#x20;
* Performing Arts&#x20;
* Post Office&#x20;
* Pre-school / Day Care&#x20;
* Restaurant&#x20;
* Retail Store&#x20;
* Senior Care Facility&#x20;
* ~~Single Family Home~~ _<mark style="color:green;">(only available via API)</mark>_
* Stadium&#x20;
* Transit Station&#x20;
* University/College&#x20;
* Worship Facility&#x20;
* Warehouse&#x20;
* Zoo

</details>

### Building Floor Area

**Number of above ground floors**

The number of building floors above grade. These floors will be assessed using the selected structural system.

**Floor area per above ground floor**

The area, in square feet, of the average aboveground floor. To determine cladding and roof area, the floor is always assumed to be square.

**Number of below ground floors**

The number of building floors below grade. These floors will be assessed as having a reinforced concrete structural system.

**Floor area per below ground floor**

The area, in square feet, of the average belowground floor. The floor is always assumed to be square.

### Site and Landscaping

**Previously developed site?**&#x20;

If the site is not previously developed, it is a greenfield site and the project incurs an emissions penalty for the site disturbance. The magnitude of this penalty is equivalent to the site area’s sequestration potential with low-sequestration plantings.

**Site Area**

The total site area (building and landscaping). To accommodate the base case building, the site area should not be lower than the average aboveground floor area.

**Planted Area**

The planted area located outside the building's footprint. This input cannot be less than the site area less the average aboveground floor area. All unplanted area is assumed to be hardscape.&#x20;
