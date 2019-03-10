# Data description
This project will require data both from field experiments and from public databases. Running the crop model requires a variety of inputs including: 1) information about soil characteristics, soil texture, clay percent; 2) information about the height of the groundwater table; 3) climate data, minimum and maximum temperature, daily precipitation, incoming radiation, atmospheric CO2 levels, latitude for calculation of solar radiation; 4) Individual crop parameters, planting date, degree days to maturity, duration of each crop growth stage, temperature range for growth, minimum and maximum rooting depth, water productivity. Water and salinity stress thresholds, minimum and maximum stomatal conductance rates, 5) Crop market values for economic assessment, expected leasing payments for farmers to lease land for solar panels to energy providers

All data manipulation or analysis will be completed using MATLAB software, all model outputs in Text format will be converted to csv for data analysis. 

Expected volume of data collected is greater than 1TB when considering the data from multiple model runs

Soil Data:

| Data Point|	Unit|	Collection Method| Collection Frequency|	Data Type|
|----------|-----|------------------|----------------------|----------|
|Soil Texture|	[-]|	Was collected onsite by previous students|	Once|spreadsheet|
|Soil PH|	pH|	Was collected onsite by previous students|	Once|	spreadsheet|
|Soil Organic| Content	kg organic matter/ kg soil| 	Was collected onsite by previous students|	Once|	spreadsheet|
|Initial soil water content|	m3 water/ m3 soil|	Will be collected via neutron probe|	Once|	spreadsheet|
|Soil water content|	m3/ m3|	Will be collected via neutron probe|	3 times a week|	spreadsheet|

Climate Data: 

| Data Point|	Unit|	Collection Method| Collection Frequency|	Data Type|
|----------|-----|------------------|----------------------|----------|
|Max. Temperature|	C|	Onsite Weather Station|	Once every minute (daily Max recorded)|	spreadsheet|
|Min. Temp	|C	|Onsite Weather Station	|Once every minute (daily min recorded)|	spreadsheet|
|Wind Speed|	Km/h|	Onsite Weather Station	Once| every minute|	spreadsheet|
|Solar Radiation	|MJ/(m2 day)	|Onsite Weather Station|	Once every minute|	spreadsheet|
|Relative Humidity|	[-]	|Onsite Weather Station|	Once every minute|	spreadsheet|
|Atmospheric C02|	ppm|	Online repository |	Once|	spreadsheet|

Crop Data:

| Data Point|	Unit|	Collection Method| Collection Frequency|	Data Type|
|----------|-----|------------------|----------------------|----------|
|Management practices (planting date, harvest date, fertilizer applied, mulch applied)|	Multiple	|Management decision|	Once	|spreadsheet|
|Irrigation amounts|	m3|	Managment decision|	Daily|	spreadsheet|
|Crop Canopy Cover|	[-]|	Overhead photograph	|3 times a week|	Photograph, information converted to a % via image analysis software then stored in spreadsheet|
|Above ground biomass|	kg	|Scale |	3 times. Twice during growth, once after harvest|	spreadsheet|
|Yield|	kg	|Scale| 	Once, after harvest|	spreadsheet|
|Dry yield	|kg|	Scale|	once, crops heated in oven to evaporate any water content|	spreadsheet|
|Stomatal Conductance|	mmol m⁻² s⁻¹|	Leaf porometer	|Variable – multiple times a week	|spreadsheet|

Economic Data:

| Data Point|	Unit|	Collection Method| Collection Frequency|	Data Type|
|----------|-----|------------------|----------------------|----------|
|Crop price|	$	|Online repository|	Once	|spreadsheet|
|Lease price for placing solar panels on land|	$	|Online repository	|Once	|spreadsheet|
|Cost of inputs|	$	|Enterprise budgets|	Once|	spreadsheet|

Output Data: 

| Data Point|	Unit|	Collection Method| Collection Frequency|	Data Type|
|----------|-----|------------------|----------------------|----------|
|Crop above ground biomass|	kg|	AquaCrop model output|	Daily|	Text file|
|Crop yield 	|kg	|AquaCrop model output	|Daily	|Text file|
|Simulated Soil water content|	m3/m3|	AquaCrop model output|	Daily	|Text file|
|Total water used per cycle	|m3	|sum daily irrigation value|	Once	|spreadsheet|
|simulated crop canopy cover|	[-]|	AquaCrop model output|	Daily	|Text file|
|Water Use Efficiency	|kg crop/m3 water	|calculation from aquacrop model results	|Once	|Text file|


# Roles and responsibilities
The general Data management roles are listed below. 
Data Collection Field experiments: Kyle Proctor
Archiving field data: Kyle Proctor
Instrumentation Maintenance: Kyle Proctor
Data Collection from online repositories: Kyle Proctor
Data Analysis/organization to prepare it for Model: Kyle Proctor
Model Data Generation: Kyle Proctor
Archiving and Preservation: Kyle Proctor + P.I. ( Kyle Proctor will be responsible for organizing all of the results into an easy to access format which he will then give to me PI and he will ensure it is preserved)

The success of this project is dependent on neither of the people with data management roles leaving the project. 

# Data standards and metadata
The AGROVOC metadata vocabulary will be used, it was developed by the Food and Agriculture Organization (FAO) who also developed the AquaCrop model that will be using for data analysis. AGROVOC is available as an SKOS-XL concept scheme. The SKOS (Simple Knowledge Organization System) is a common data model for sharing and linking information. The use of this metadata standard should improve the overall long term utility and reproducibility of the work.  


# Storage and security
All data will be stored on the OSU Biological and Ecological Engineering (BEE) server using version control via TortoiseSVN software for the duration of the project. Thus two copies of the data will exist, one on a desktop hard drive and one on the department server. The data can remain on this server for the extent of the main author’s doctoral process. Following completion of the doctorate, the data crucial to the project will be stored in the ScholarsArchive along with the thesis. At this point further determinations need to be made about external locations for storing this data.

Since such a large volume of data is being collected daily it will be important to systematically store the data. The plan is to download the climate data once a week and then store each of these files as its own excel sheet, data will be extracted and aggregated from these excel sheets for data analysis but the raw data will not be changed.

For crop variables, measurements of biomass and yield will be weighed in the field and recorded manually on paper, this paper will be photographed and then this information will transferred to a spreadsheet, once again information will be extracted and aggregated from the excel sheet but the raw data will not be changed

Measurements of crop canopy cover require overhead photographs of the crops as they grow, these photographs are then analyzed using image analysis software to determine what proportion of the ground is covered by the plant canopy, these photographs will be dated and stored along with a spreadsheet cataloguing the numerical percentages of ground covered. 

All collected data will eventually be partitioned into calibration and validation sets for the crop growth model, the method of this data partitioning has not yet been determined.


# Access and data sharing
There are no limits on the ability to share data from this research. No sensitive information will be present. The data will be made publically available at either the time of the first journal publication using this work or when the doctoral thesis is submitted, whichever comes first.  Depending on the volume of data it will either be published separately as a data paper or available in the supplementary materials of the journal publication. Data will be made available in the form of csv spreadsheets, if the model results are extrapolated geographically (ex. calculating model yield in the entire Willamette valley instead of at one point) that data would be published as a GIS shape file with corresponding tables embedded

In the short term, data will be preserved on both the OSU Biological and Ecological Engineering’s server and on a desktop hard drive following completion of the experiments the data may be submitted to a data repository such as the WOLFRAM Data repository under the Agriculture category. The data will also be stored in the Oregon State Scholar’s Archive along with the doctoral thesis discussing the work. For long term archiving all data will be stored in the form of csv spreadsheets except for model results extrapolated geographically which will be stored as a GIS shape file as discussed above.


# Archiving and preservation
Specifics on the methods of data archival are discussed in the section above. Access to the archived data will be maintained by the respective organizations, the repository data is submitted too and the OSU Scholar’s Archive. It is always difficult to be sure how long data will be maintained but the OSU Scholar’s archive pledges to maintain and preserve the content and metadata and also provides a persistent URL that will not break or disappear. The stored data will be in the form of csv spreadsheets.
