# <p align="center"> TecNav
<p align="center">
<b>Clinic-Monitoring & Technician-Navigation Application</b>
</p>
<p align="center">
  <img 
    width="550"
    height="350"
    src="https://user-images.githubusercontent.com/79323360/170838284-edba9418-8f2b-4ca1-a880-db3651fbe247.png"
  >
</p>
<p align="center">
Romith Challa</b>
Tomer Danon</b>
Data Science Capstone</b>
University of Denver</b>
</p>

## <p align="center"> Executive Summary
According to a 2019 benchmark report from the Urgent Care Association, the number of urgent-care clinics increased by 9.6% from the previous year. As the pandemic continues to put a strain on the healthcare system, the appeal for convenient and affordable care-outlets is greater than ever. To meet this growing need for on-demand care, urgent-care clinics have been rapidly expanding the scope of their services to provide patients with a quick and affordable alternative to the emergency room. This proves to be a mutually exclusive endeavor as minimizing wait-times entails maximizing staff availability. Consequently, this leads to higher operational costs that eventually trickle down to patient bills. Due to the inconsistency in patient traffic, it is difficult to schedule staff to be able to handle the peak hours, without inevitably wasting resources during less busy hours. Some chain-operated clinics creatively handle this by transferring technicians between their various locations to account for the constantly evolving needs at each clinic. This requires continuous monitoring of each clinic to manually make navigation decisions based on the fluctuating patient traffic. Instead, a software application that streamlines this process to make real-time, data-driven navigation decisions would serve as an invaluable tool for these clinics. That is the motivation behind TecNav—an automated application that employs machine-learning to forecast the dynamic patient flow and navigate technicians without any human supervision. Based on the preliminary results of the prototype, TecNav can save clients over $90,000 for each clinic per year. This could potentially finance their mission to expand clinical services, without burdening patients with higher costs. Designed with an emphasis on translatability, TecNav’s algorithm is customizable to fit the needs of any potential client.

## Usage
- <b>uc_data_fabricator.ipynb</b>: As there are no publicly-available datasets that fit the scope of this project, this notebook will execute a series of data fabrication steps to generate datasets to emulate the real-world as much as possible. To aid this process, secondary research was relied upon to to strategize the approach at each level. These datasets will serve as the raw data source down the project pipeline. <b>NOTE</b> - fabricated_data folder contains the generated datasets. The notebooks mentioned below are setup to use this pre-fabricated data without the need to run uc_data_fabricator.ipynb.
- <b>uc_eda.ipynb</b>: This notebook will explore the generated datasets to draw insights from the patient visits and any relationships between date/times to inform the modeling and navigation process. <b>NOTE</b> - Not all visual outputs are pre-loaded. For best visual output and to utilize the interactive toggle-menu for plots, execute this script in a Jupyter notebook (VS-Code does not fully support .ipynb interactive widgets).
- <b>uc_modeler.ipynb</b>: This notebook will construct and evaluate baseline models to help select a decision-maker within the navigation software.
- <b>uc_analysis.ipynb</b>: This notebook will implement technician-navigation to study the potential benefits in productivity and operational costs. This notebook utilizes uc_navigator.py and TecNav_Demo.py.
- <b>uc_navigator.py</b> (for reference only): Contains navigator application. This module is launched within uc_analysis.ipynb.
- <b>TecNav_Demo.py</b> (for reference only): Contains demo dashboard application. This module is launched within uc_analysis.ipynb.
