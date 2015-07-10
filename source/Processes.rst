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


Central level MOS
------------------
**Central level MOS** = **Stock on Hand at central level** / **Adjusted facility AMC**
	where;

	*Stock on Hand (SOH)* : This is the total quantity held in stock at the central level - as reported by the supply chain agency (KEMSA).

	Total Monthly Consumption (TMC) at Facility level is obtained by summing the quantity dispensed (across all facilities in the country). This monthly TMC is adjusted to cater for non-reporting facilities to obtain the adjusted facility AMC using the formula:

		**Adjusted facility AMC** = {[(TMCN1/NMRR1)+(TMCN2/NMRR2)+(TMCN3/NMRR3)+...+(TMCN*n*)] / *n*}

 





.. toctree::
    :maxdepth: 3
