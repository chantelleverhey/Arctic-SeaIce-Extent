# README

This repository was created as part of a final project for 5803 - Geomatics class at Carleton University. The exercise is meant to be used in conjunction with the 'Open-SeaICE-Extent' repository which does a more basic walk through demonstration of how to take advantage of the 'open data movement' when it comes to analyzing sea-ice extent in the arctic

For the purpose of this repository - we have done a more indepth analysis of sea-ice extent of the Arctic and then broken it down a stage lower at the regional level, and finally, with a community level example. 

The following outlines the data sources for each level
- Pan-Arctic: NSIDC --> Sea_Ice_Index_Monthly_Data_by_Year_G02135_v3.0-extent.csv
- Regional: NSIDC --> N_Sea_Ice_Index_Regional_Monthly_Data_G02135_v3.xlsx dataset
- Local: This walkthrough was a demonstration of reuse of an existing jupyter notebook from Eurodata Cube 'USING SENTINEL HUB PYTHON PACKAGE IN EDC: A STARTER'S GUIDE' repurposed for a usecase in Pond Inlet, Baffin bay, Nunavut, Canada
https://eurodatacube.com/notebooks

Acronyms:
SIE- Sea-ice Extent
NSIDC - National Snow and Ice Data Centre
LCC - Lowest Cloud Coverage
S2A - Sentinel 2A (Sentinel Hub)
4b - 4 band image

The following are the file structures in Arctic-SeaIce-Extent Repository:

- README (this file)

- Arctic-SIE
    - NSIDC-Arctic-SIE.jpynb
    - Sea_Ice_Index_Monthly_Data_by_Year_G02135_v3.0-area
    - Sea_Ice_Index_Monthly_Data_by_Year_G02135_v3.0-extent

- Local-SIE
    - Pond-Example-Image.ipynb
    - Arctic-SeaIce-Extent/Local-SIE/Pond-SeaIce-Images
        - 15Sept2023-S2A-4b.png
        - 15Sept2023-S2A.png
        - 16May2020-S2A-4b.png
        - 16May2020-S2A.png
        - May2018-S2A-LCC.png
        - May2019-S2A-LCC.png
        - May2020-S2A-LCC.png
        - May2021-S2A-LCC.png
        - May2022-S2A-LCC.png
        - May2023-S2A-LCC.png
        - Sept2023-S2A-LCC.png

- Regional-SIE
    - README-Regional.md
    - Regional-SIE-Timeseries.ipynb
    - Baffin-SIE-km2.csv
    - Barents-SIE-km2.csv
    - Beaufort-SIE-km2.csv
    - Bering-SIE-km2.csv
    - CArchi-SIE-km2.csv
    - CArctic-SIE-km2.csv
    - Chukchi-SIE-km2.csv
    - Esiberia-SIE-km2.csv
    - Greenland-SIE-km2.csv
    - Hudson-SIE-km2.csv
    - Kara-SIE-km2.csv
    - Laptex-SIE-km2.csv
    - Okhotsk-SIE-km2.csv
    - StLawrence-SIE-km2.csv
    

    
Licensing: CC-BY
This license enables reusers to distribute, remix, adapt, and build upon the material in any medium or format, so long as attribution is given to the creator. The license allows for commercial use.
