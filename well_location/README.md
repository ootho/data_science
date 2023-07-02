# Well Location Selection

[View Notebook](https://nbviewer.org/github/ootho/data_science/blob/main/well_location/well_location.ipynb)

## Project Objective and Tasks

The dataset contains samples of oil from three regions, with 10,000 oil wells in each region. The quality of oil and the volume of reserves were measured for each well. The goal is to build a machine learning model that will help determine the region where drilling will bring the highest profit. It is necessary to analyze the potential profit and risks.

**Tech Stack: Python, Pandas, Scikit-learn**

## Conclusion

The following steps were taken during the project:
- Data preparation: unnecessary columns were removed, features were scaled, and data types were optimized.
- A linear regression model was trained and its results were analyzed.
- The minimum oil reserves required for profitable well development were calculated.
- The average profit and risks of losses were calculated using the bootstrap method.
- Based on the results, a region for well development was recommended, and justified recommendations were provided.