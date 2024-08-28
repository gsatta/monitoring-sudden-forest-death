![logo_app_github](https://github.com/user-attachments/assets/3eb64167-c84e-4291-b490-274e9b07703d)

# Monitor and Quantify Sudden Forest Death in Sardinia.
This repository provides tools to analyze and monitor [Sudden Forest Death in Sardinia](https://www.ildolomiti.it/altra-montagna/ambiente/2024/crisi-dei-boschi-in-sardegna-la-regione-stanzia-oltre-un-milione-di-euro-per-individuare-soluzioni-e-incrementare-il-monitoraggio?fbclid=IwY2xjawE8BqFleHRuA2FlbQIxMQABHdW1rBfI_5mGb-H0-TFj_Sw0if4RmvzGPNbVCG8U65dgW_ISv2t79afK4A_aem_xziHfAe9isCuQji6C3Ir0Q) in Sardinia using satellite imagery and vegetation indices. 
The application integrates data from Sentinel-2 and other Earth Engine datasets to visualize and quantify areas where forest decline has been detected.



## How it works?
0. **User Interface**: Users can adjust cloud coverage thresholds and input different date ranges through an intuitive UI. Results are displayed on the map with a custom legend.
1. **Data Selection**: Users can select two date ranges to compare vegetation health over time. The application uses cloud-filtered Sentinel-2 imagery for the selected periods.
2. **Tree Coverage Detection**: The script filters for high-probability tree coverage, generating a binary tree mask based on Dynamic World’s tree probability layer.
![image](https://github.com/user-attachments/assets/96b24bae-6156-4e65-bd59-80b9fa314934)

4. **Normalized Green Red Difference Index (NGRDI)**: The app calculates the NGRDI for both selected periods to highlight changes in vegetation health.
5. **Delta NGRDI Calculation**: A change detection algorithm computes the difference between NGRDI values of the two time intervals. Negative differences indicate vegetation decline.
6. **Patches Identification**: Areas with significant vegetation loss (ΔNGRDI < -0.1) are identified and visualized. These patches are also filtered by size, retaining only areas larger than 1 hectare.
7. **Total Affected Area Calculation**: The total area of forest loss is calculated and displayed in hectares.

![image](https://github.com/user-attachments/assets/93312beb-675d-4c1f-95f0-aa0092d64ef8)


This repository provides tools, methods, and resources to help researchers, ecologists, and forestry professionals detect and monitor the alarming phenomenon of Sudden Forest Death, particularly in the forests of Sardinia.





