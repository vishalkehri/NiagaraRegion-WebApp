# NiagaraRegion-WebApp
The web application was created for Niagara Region named Market Research Analyst is a website that is a single source of data collection and holds the land use, transit, demographic, and schools data of 4 municipalities. The intent is to provide the data to new business investors/stakeholders to collect, manipulate, and analyze data to determine the business opportunities in the region. Earlier, the data was collected separately from all the municipalities however, now all the required data is avaialble on this application.

# Problem
Niagara Region consists of 12 municipalities and the data exists in various formats and needs to be collected from each municipal office/website individually. Data accessibilty issues were being faced by the new business investors/stakeholders to perform analysis for the opportunities.

# Solution
The web mapping application is a one stop shop for the investors/stakeholders to access the data of different municipalities in the most commonly used formats. Hassle is gone to visit each municipality office/website.

# Process
The application was published on ArcGIS Online platform using FME (Feature Manipulation Engine). The process is as follows:
- Read the data in FME using suitable readers for the given format.
- Managed attributes through attribute manager to define type of attributes and create aliases for the end user.
- Created attributes to add data for better understanding of the end user.
- Filtered the land use data based on the land use codes as per each municipal plan.
- Converted the filtered land use data to land use feature classes in the final geodatabase.
- Similar procedure was followed to normalize transit and school data.
- Demographic data was filtered based on age groups and income groups using the attribute manager.
- All data tables were joined using the land use code as primary key where the end user can access all data for a particualt land use parcel in the region.
- The geodatabase was published to ArcGIS Online service.
- Web Application was equipped with the tools to create, buffer, clip, and download the data in Excel, CSV, and Shapefile formats.
