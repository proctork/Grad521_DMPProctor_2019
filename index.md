# Data description
This project will require data both from field experiments and from public databases. Running the crop model requires a variety of inputs including: 1) information about soil characteristics, soil texture, clay percent; 2) information about the height of the groundwater table; 3) climate data, minimum and maximum temperature, daily precipitation, incoming radiation, atmospheric CO2 levels, latitude for calculation of solar radiation; 4) Individual crop parameters, planting date, degree days to maturity, duration of each crop growth stage, temperature range for growth, minimum and maximum rooting depth, water productivity. Water and salinity stress thresholds, minimum and maximum stomatal conductance rates, 5) Crop market values for economic assessment, expected leasing payments for farmers to lease land for solar panels to energy providers

All data manipulation or analysis will be completed using MATLAB software, all model outputs in Text format will be converted to csv for data analysis. 

Expected volume of data collected is greater than 1TB when considering the data from multiple model runs



# Roles and responsibilities
The general Data management roles are listed below. 
Data Collection Field experiments: Kyle Proctor
Archiving field data: Kyle Proctor
Instrumentation Maintenance: Kyle Proctor
Data Collection from online repositories: Kyle Proctor
Data Analysis/organization to prepare it for Model: Kyle Proctor
Model Data Generation: Kyle Proctor
 Archiving and Preservation: Kyle Proctor + P.I. (I will be responsible for organizing all of my results into an easy to access format which I will then give to me PI and he will ensure it is preserved)
The success of this project is dependent on neither of the people with data management roles leaving the project. 


# Data standards and metadata
The AGROVOC metadata vocabulary will be used, it was developed by the Food and Agriculture Organization (FAO) who also developed the AquaCrop model that will be using for data analysis. AGROVOC is available as an SKOS-XL concept scheme. The SKOS (Simple Knowledge Organization System) is a common data model for sharing and linking information. The use of this metadata standard should improve the overall long term utility and reproducibility of the work.  



# Storage and security
All data will be stored on the OSU Biological and Ecological Engineering (BEE) server using version control via TortoiseSVN software for the duration of the project. Thus two copies of the data will exist, one on a desktop hard drive and one on the department server. The data can remain on this server for the extent of the main author’s doctoral process. Following completion of the doctorate, the data crucial to the project will be stored in the ScholarsArchive along with the thesis. At this point further determinations need to be made about external locations for storing this data.
Since such a large volume of data is being collected daily it will be important to systematically store the data I plan to download the climate data once a week and then store each of this files as its own excel sheet, data will be extracted and aggregated from these excel sheets for data analysis but the raw data will not be changed.
For crop variables, measurements of biomass and yield will be weighed in the field and recorded manually on paper, this paper will be photographed and then this information will transferred to a spreadsheet, once again information will be extracted and aggregated from the excel sheet but the raw data will not be changed
Crop canopy cover requires overhead photographs of the crops as they grow, these photographs are then analyzed using image analysis software to determine what proportion of the ground is covered by the plant canopy, these photographs will be dated and stored along with a spreadsheet cataloguing the numerical percentages of ground covered. 
All collected data will eventually be partitioned into calibration and validation sets for the crop growth model, the method of this calibration has not yet been determined.


# Access and data sharing
 There are no limits to the availability to share data from this research. No sensitive information will be present. The data will be made publically available at either the time of the first journal publication using this work or when my doctoral thesis is submitted, whichever comes first.  Depending on the volume of data it will either be published separately as a data paper or available in the supplementary materials of the journal publication. Data will be made available in the form of csv spreadsheets, if the model results are extrapolated geographically (ex. calculating model yield in the entire Willamette valley vs one point) that data would be published as a GIS shape file with corresponding tables embedded
In the short term data will be preserved on both the OSU Biological and Ecological Engineering’s server and on a desktop hard drive following completion of the experiments the data may be submitted to a data repository such as the WOLFRAM Data repository under the Agriculture category. The data will be stored as in the Oregon State Scholar’s Archive along with the doctoral thesis discussing the work. For long term archiving all data will be stored in the form of csv spreadsheets except for model results extrapolated geographically which will be stored as a GIS shape file as discussed above.

# Archiving and preservation
Specifics on the methods of data archival are discussed in the section above. Access to the archived data will be maintained by the respective organizations, the repository data is submitted too and the OSU Scholar’s Archive. It is always difficult to be sure how long data will be maintained but the OSU Scholar’s archive pledges to maintain and preserve the content and metadata and also provides a persistent URL that will not break or disappear. The stored data will be in the form of csv spreadsheets
