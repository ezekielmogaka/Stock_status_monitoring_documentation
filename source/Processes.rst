Processes
==========

Procceses involved
-------------------


After the capture of the monthly transaction data, the tool calculates the MOS data for facility, county and central levels.
The basic formula for **months of Stock (MOS)** is:

	*Months of Stock(MOS)* = *Stock on Hand (SOH)* / *Average Monthly Consumption(AMC)*


Months of Stock (MOS) is normally stored as a number, with one decimal point.
Stock on Hand (SOH) is captured as an absolute figure based on Physical Stock Count or a Warehouse report. SOH is reported at different levels of the supply chain:

	- Central level
	- County level
	- Facility level

Average Monthly Consumption (AMC) is captured only at facility level (where consumption happens), and may be adjusted for reporting rateto cater for consumption at non-reporting facilities.

MOS is computed at four levels:

	#. Central level 
	#. Facility level
	#. National level
	#. County level


Central Level MOS
------------------
**Central level MOS** = **Stock on Hand at central level** / **Adjusted facility AMC**
	where;

	*Stock on Hand (SOH)* : This is the total quantity held in stock at the central level - as reported by the supply chain agency (KEMSA).

	*Total Monthly Consumption (TMC)* at Facility level is obtained by summing the quantity dispensed (across all facilities in the country). This monthly TMC is adjusted to cater for non-reporting facilities to obtain the adjusted facility AMC using the formula:

		**Adjusted facility AMC** = {[(TMCN1/NMRR1)+(TMCN2/NMRR2)+(TMCN3/NMRR3)+...+(TMCNn)] / *n*}

		where;

		**TMCN** = Total Monthly Consumption National Level. Its obtained by aggregating repored total quantity dispensed across all facilities in the country. (Data from DHIS2).

		**NMRR** = National Monthly Reporting Rate expressed as a percentage (Data from DHIS2).

		**n** = Number of months(Typically six months).

	Central level MOS is computed for all commodities.


Facility Level MOS
--------------------
**Facility Level MOS** = **Total Stock on Hand at Facility level** / **Adjusted facility AMC**

	where;
	*Total Stock on Hand at Facility level*: is the total quantity held in stockin health facilities across the country. It is obtained by aggregating the physical stock count across all facilities in the country. (Data from DHIS2).


	**Adjusted facility AMC** is given by the formula below:

	**Adjusted facility AMC** = {[(TMCN1/NMRR1)+(TMCN2/NMRR2)+(TMCN3/NMRR3)+...+(TMCNn)] / *n*}

	**TMCN** = Total Monthly Consumption National Level. Its obtained by aggregating repored total quantity dispensed across all facilities in the country. (Data from DHIS2).

		**NMRR** = National Monthly Reporting Rate expressed as a percentage (Data from DHIS2).

		**n** = Number of months(Typically six months).

	Facility level MOS is computed for all commodities.


National Level MOS
--------------------
National level MOS is obtained by summing the Central Level MOS and the Facility Level MOS
**National Level MOS** = **Central Level MOS + Facility Level MOS**

National Level MOS is computed for each commodity.


County Level MOS
--------------------
**County Level MOS** = **Total Stock on Hand at County level** / **Adjusted county AMC**

	where;
	*Total Stock on Hand at County level*: is the total quantity held in stock in the county. It is obtained by aggregating the physical stock count across all facilities in the county. (Data from DHIS2).


	**Adjusted County AMC** is given by the formula below:

	**Adjusted County AMC** = {[(TMCC1/NMRR1)+(TMCC2/NMRR2)+(TMCC3/NMRR3)+...+(TMCCn)] / *n*}

	**TMCC** = Total Monthly Consumption County Level. Its obtained by aggregating repored total quantity dispensed across all facilities in the county. (Data from DHIS2).

	**NMRR** = National Monthly Reporting Rate expressed as a percentage (Data from DHIS2).

	**n** = Number of months(Typically six months).

	County level MOS is computed for each county for all commodities.

Using the processes/formulas provided above, the tool should produce the outputs shown below:





.. toctree::
    :maxdepth: 3
