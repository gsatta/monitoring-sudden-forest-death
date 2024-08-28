![logo_app_github](https://github.com/user-attachments/assets/1aa95f5e-cbc8-4c77-86cc-174a81344de0)<img class="aligncenter size-full wp-image-8747" alt="markdown" >

# Monitor and Quantify Sudden Forest Death in Sardinia.
This repository provides tools to analyze and monitor Sudden Forest Death (SFD) in Sardinia using satellite imagery and vegetation indices. 
The application integrates data from Sentinel-2 and other Earth Engine datasets to visualize and quantify areas where forest decline has been detected.


**How it works?**
Data Selection: Users can select two date ranges to compare vegetation health over time. The application uses cloud-filtered Sentinel-2 imagery for the selected periods.
Tree Coverage Detection: The script filters for high-probability tree coverage, generating a binary tree mask based on Dynamic World’s tree probability layer.
Normalized Green Red Difference Index (NGRDI): The app calculates the NGRDI for both selected periods to highlight changes in vegetation health.
Delta NGRDI Calculation: A change detection algorithm computes the difference between NGRDI values of the two time intervals. Negative differences indicate vegetation decline.
Patches Identification: Areas with significant vegetation loss (ΔNGRDI < -0.1) are identified and visualized. These patches are also filtered by size, retaining only areas larger than 1 hectare.
Total Affected Area Calculation: The total area of forest loss is calculated and displayed in hectares.
User Interface: Users can adjust cloud coverage thresholds and input different date ranges through an intuitive UI. Results are displayed on the map with a custom legend.z

This repository provides tools, methods, and resources to help researchers, ecologists, and forestry professionals detect and monitor the alarming phenomenon of Sudden Forest Death, particularly in the forests of Sardinia.


![image](https://github.com/user-attachments/assets/96b24bae-6156-4e65-bd59-80b9fa314934)



![image](https://github.com/user-attachments/assets/93312beb-675d-4c1f-95f0-aa0092d64ef8)
