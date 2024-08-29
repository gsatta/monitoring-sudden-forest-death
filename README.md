![logo_app_github](https://github.com/user-attachments/assets/2f6e5990-bcfa-4db0-99d7-2de8fe818c9a)

# Monitor and Quantify Sudden Forest Death in Sardinia.
This repository provides information about an [app](https://ee-sattagabrielega2.projects.earthengine.app/view/monitoraggiomoriaquerce) developed to analyze and monitor [Sudden Forest Death in Sardinia](https://www.ildolomiti.it/altra-montagna/ambiente/2024/crisi-dei-boschi-in-sardegna-la-regione-stanzia-oltre-un-milione-di-euro-per-individuare-soluzioni-e-incrementare-il-monitoraggio?fbclid=IwY2xjawE8BqFleHRuA2FlbQIxMQABHdW1rBfI_5mGb-H0-TFj_Sw0if4RmvzGPNbVCG8U65dgW_ISv2t79afK4A_aem_xziHfAe9isCuQji6C3Ir0Q) using satellite imagery and vegetation indices. 
The application integrates data from Sentinel-2 and other Earth Engine datasets to visualize and quantify areas where forest decline has been detected.

## How it works?
0. **User Interface**: Users can adjust cloud coverage thresholds and input different date ranges through an intuitive UI. Furthermore users can select the regions of interest (Sarinia or Corsica). Results are displayed on the map with a custom legend.
1. **Data Selection**: Users can select two date ranges to compare vegetation health over time. The application uses cloud-filtered Sentinel-2 imagery for the selected periods. **It is important that the two date ranges are not too wide.**
2. **Tree Coverage Detection**: The script filters for high-probability tree coverage, generating a binary tree mask based on [Dynamic World’s](https://dynamicworld.app/) tree probability layer. Reducing the threshold increases the area in which the analysis is carried out, including other areas that are not properly forest.
   
![image](https://github.com/user-attachments/assets/f23d1167-45bb-4233-a38b-809247dd9b22)

4. **Normalized Green Red Difference Index (NGRDI)**: The app calculates the [NGRDI](https://www.indexdatabase.de/db/i-single.php?id=390) for both selected periods to highlight changes in vegetation health.
5. **Delta NGRDI Calculation**: A change detection algorithm computes the difference between NGRDI values of the two time intervals. Negative differences indicate vegetation decline.
6. **Patches Identification**: Areas with significant vegetation loss (ΔNGRDI < -0.1) are identified and visualized. These patches are also filtered by size, retaining only areas larger than 1 hectare.
7. **Total Affected Area Calculation**: The total area of symptomatic forest is calculated and displayed in hectares.

![image](https://github.com/user-attachments/assets/9574c884-51df-4f78-bd8e-88205f8f13e1)

In conclusion this repository provides tools, methods, and resources to help researchers, ecologists, and forestry professionals detect and monitor the alarming phenomenon of Sudden Forest Death, particularly in the forests of Sardinia.

## How to use it?

![image](https://github.com/user-attachments/assets/f43a0ba5-10c0-40e8-ba97-55025029914e)



**The app is still in progress !**

![image](https://www.colibriensemble.it/wp-content/uploads/2018/07/Work-in-Progress.png)






