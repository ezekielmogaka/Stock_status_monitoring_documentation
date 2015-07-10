Data setup by the tool
===============================================

Master Data Setup
------------------


- **Funding agencies** - allows setup of various funding agencies that provide malaria commodities. This tool is dynamic in nature therefore allows continuous addition of funding sources as and when required.

	The following details of the funding agenciies are captured:
		#. Funding agency e.g GoK, UNITAD, PMI etc..
		#. Comment about the funding agency

- **Supply Chain Agencies**- allows setup of supply chain agencies that receive and issue malaria commodities. The tool allows for continuous addition of funding sources when required.
	The following information about Supply chain agencies is captured:
		#. Supply Chain agency e.g KEMSA
		#. Comment about the spply chain agencies
		#. Contact person
		#. Contact phone



- **List of Malaria Zones** -The tool allows for the setup of malaria zones.
	The following information about malaria zones is captured:
		#. Zone e.g Zone 1 : Endermic
		#. Comment about the malaria zone
		


- **List of counties** - The tool allows for the setup of counties information.
	The following information about counties is captured:
		#. Name of county e.g Muranga
		#. Comment about the county
		#. Zone e.g Epidermic

- **Malaria commodities data** -The tool allows setting up of Malaria commodities being tracked (AL 6s, AL 12s, AL 18s, AL24s, RDTs, Artesunate injection). The tool has easy capability of adding malaria commodities. The list of commodities generated is used in subsequent data capture sections.
	The following information is captured:
		#. Commodity name
		#. Unit of measure
		#. Name of funding agency - It is picked from the list of funding sources

- **Commodity level Data** -This tool allows for the following information to be defined:
		#. Forecast period(number of years that the forecast covers)
		#. Forecast start date
		#. Forecast Monthly consumption for each commodity(obtained from the quantification report). This is entered for every month acrss the forecast period.


Information captured by the tool
---------------------------------

	#. **Central level Data** - Central level stock on hand (SOH). This information reflects the status of stock at central level and is received from KEMSA on a monthly basis. Once captured, this information is used to generate various required outputs. The central level stock on hand data is captured for each malaria commodity. Information on pending stocks as received from the supply chain agencies JSI Deliver and KEMSA is captured at this stage. 

	#. **Facility level data** - The tool allows for the capture of facility Level stock on hand for ACTs and RDTs. This information is obtained from DHIS2 and is keyed in.

	#. **County level data** - The tool allows for the capture of county Level stock on hand for ACTs and RDTs. This information is obtained from DHIS2 and is keyed in. the tool should however has provision to retrieve this data from DHIS directly.


.. toctree::
    :maxdepth: 2
