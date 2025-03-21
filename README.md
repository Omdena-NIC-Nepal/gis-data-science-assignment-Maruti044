# GIS_Data_Science
## Assignment: GIS Data Science for Climate in Nepal
### Objective:
- This assignment aims to analyze climate data for Nepal using GIS techniques. The focus is on reading, visualizing, and conducting exploratory data analysis (EDA) tasks using Python on temperature and precipitation data to identify trends and potential climate impacts. 

### Steps to Complete the Assignment:
#### Setup Instructions:

- Clone the repository from GitHub Classroom. git clone https://github.com/Omdena-NIC-Nepal/gis-data-science-assignment-Maruti044.git
- Ensure Python environment is set up with necessary libraries (e.g., pandas, geopandas, matplotlib, seaborn).
#### Data Collection and Preparation:

- Data Source: Use climate-related GIS data for Nepal. https://github.com/Desmondonam/Nepal_Climate_change
### Dataset Contents
    -	Shapefiles (local_unit.shp): Contains Nepal's administrative boundaries.
    -GeoPackage Files (.gpkg):
        nepal_admin_regions.gpkg: Administrative boundaries.
        nepal_glaciers.gpkg: Glacier regions.
        nepal_rivers.gpkg: River networks.
    -TIFF Files (.tif):
        nepal_temperature_2020.tif: Temperature data for 2020.
        nepal_temperature_2050.tif: Projected temperature for 2050.
        nepal_precipitation_2020.tif: Precipitation data for 2020.
        nepal_precipitation_2050.tif: Projected precipitation for 2050.
### Preprocessing Steps
•	Read raster (TIFF) data using rasterio.
•	Load shapefile and GeoPackage data using geopandas.
•	Convert raster data into a suitable format for visualization and analysis.

## Analysis & Findings

### Key Findings from the Precipitation Change (2050 - 2020)

        -The southern and southeastern regions of Nepal show a significant decrease in precipitation (represented by red/orange shades, indicating a reduction of up to ~100 mm).
        -The northern and northwestern regions experience a relatively lower decrease or even slight increases in precipitation (represented by blue shades).
        -Potential Drying Trend in the South
        -The Terai and lower hill regions (southern Nepal) appear to be at higher risk of reduced rainfall, which may impact agriculture and water resources.
        -This trend aligns with climate projections that predict increased drought risk in lowland areas.
        -More Stable or Increasing Precipitation in the North
        -The Himalayan and high-altitude regions (northern Nepal) show less drastic reductions or slight increases in precipitation.
        -This could indicate a shift in monsoon dynamics or changes in snow accumulation patterns.
        -Implications for Agriculture & Water Resources
        -The decreasing precipitation in the south may lead to water shortages, reduced crop yields, and increased dependency on irrigation.
        -The northern regions might experience increased glacier melt, potentially causing temporary water surges followed by long-term water scarcity.
### Key Findings from the Projected Temperature Change (2050 - 2020)
       - The entire map shows positive temperature changes, with most areas experiencing an increase of 1°C to 5°C by 2050.
       - Some isolated areas appear to have minimal or negative change (-1°C), but these are rare.
        Higher Warming in the Northern Regions

        -The Himalayan and high-altitude regions (northern Nepal) show a higher temperature increase (~3°C to 5°C).
        This aligns with global climate trends, where mountainous and polar regions warm faster than lowlands.
      
        -The Terai (southern plains) and mid-hills show moderate warming (~1°C to 3°C).
        This increase may exacerbate heat stress, impact agriculture, and increase water demand.

       - Glacier Melt & Water Resources: Increased warming in the Himalayas could lead to accelerated glacier melting, impacting river flows and increasing flood risks in the short term.

        -Agriculture & Livelihoods: Rising temperatures may reduce crop yields (especially for heat-sensitive crops like wheat and rice) and increase pest infestations.

        -Human Health: Higher temperatures could increase the risk of heatwaves, vector-borne diseases, and water scarcity, particularly in the Terai region.
### Finding from tempararure distribution among administrative boundaries of Nepal
       - Temperature Gradient: There is a clear temperature gradient from the southern to the northern regions of Nepal. The southern regions (lower latitudes) are significantly warmer, represented by red and orange hues, while the northern regions (higher latitudes) are much colder, represented by blue hues.

        -Altitude Influence: The temperature pattern strongly suggests that altitude plays a significant role in temperature distribution. The warmer southern regions are generally at lower altitudes (the Terai plains), while the colder northern regions are at higher altitudes (the Himalayan mountains).

        -Regional Variations: Even within the broader temperature gradient, there are smaller variations. Some areas at similar latitudes show slightly different temperatures, indicating local factors influencing temperature (e.g., local topography, proximity to water bodies, etc.).

        -Administrative Boundaries: The map includes the boundaries of local administrative units. While these boundaries don't directly influence the temperature distribution, they provide a geographical context for understanding the temperature patterns in relation to administrative regions.

        -Temperature Scale: The temperature scale on the right side of the map ranges from approximately -20°C to +5°C. This indicates a significant temperature variation across Nepal, highlighting the diverse climate within the country.

        -Southern Plains (Terai): The southern plains show the warmest temperatures, likely due to lower altitude and subtropical climate.

       - Mid-Hills: The mid-hill regions show intermediate temperatures, transitioning from warmer to colder as altitude increases.

       - Himalayan Region: The northern Himalayan region exhibits the coldest temperatures, indicative of high altitude and alpine climate.
      
## Summary 
        Similar Medians: The medians for both 2020 and 2050 are quite close, suggesting that the central tendency of precipitation might not change drastically between the two years.

        Increased Variability in 2050: The 2050 boxplot shows a wider range of values and more outliers compared to 2020. This indicates a higher variability or spread in precipitation in 2050.

        Potential for Extreme Events in 2050: The increased number of outliers, especially on the higher end, suggests a higher likelihood of extreme precipitation events (heavy rainfall) in 2050.  The presence of outliers below 0 mm might indicate potential data anomalies or extreme drought conditions.

        Slight Decrease in Median: While the medians are close, there's a slight decrease in the median precipitation for 2050 compared to 2020.

### Overall Warming Trend
        -The mean temperature increases from -7.58°C (2020) to -5.47°C (2050), indicating an overall warming of ~2.1°C.
        -The median temperature also increases (from -7.69°C to -5.58°C), confirming a shift towards higher temperatures.
#### Higher Maximum Temperatures
    -The maximum temperature increases from 8.14°C to 11.47°C, suggesting that hotter regions will experience even more extreme temperatures.
#### Minimal Change in Coldest Areas
    -The minimum temperature changes only slightly (-23.20°C to -22.09°C), meaning the coldest areas (likely high-altitude regions) may not warm as much as lower-elevation areas.
#### Implications of Rising Temperatures
    -Accelerated glacier melting in the Himalayas, leading to potential flooding and water shortages.
    -Increased heat stress in lower regions, affecting agriculture, water resources, and human health.
    -Changes in biodiversity and ecosystems, especially in high-altitude regions.
### Precipitation Analysis
#### Slight Decline in Average Precipitation
    -The mean precipitation decreases from 50.84 mm (2020) to 48.29 mm (2050), showing a ~2.5 mm reduction in rainfall on average.
    -The median precipitation also drops (50.37 mm to 46.74 mm), meaning that overall, Nepal is expected to receive slightly less rainfall.
#### More Extreme Rainfall Variability
    -Maximum precipitation increases from 102.83 mm to 134.97 mm, indicating that some areas might experience heavier rainfall events.
    -Minimum precipitation drops from 6.86 mm to -6.41 mm, suggesting that some regions might see periods of drought or drastic reduction in rainfall.
#### Implications of Changing Rainfall Patterns
    -Higher risk of extreme weather events (floods & droughts) due to increased variability.
    -Potential agricultural disruptions, as some regions might suffer from both excessive rain and dry spells.
    -Impact on water resources, affecting drinking water supply, irrigation, and hydropower generation.
