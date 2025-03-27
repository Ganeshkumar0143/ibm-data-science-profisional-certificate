# ibm-data-science-profisional-certificate
SpaceX Falcon 9 Landing Prediction
Overview
This project aims to predict the success of SpaceX Falcon 9 first-stage landings using data analysis and visualization techniques. SpaceX advertises Falcon 9 rocket launches at a cost of $62 million, significantly lower than competitors (upward of $165 million), largely due to the reusability of the first stage. By determining whether the first stage will land successfully, we can estimate launch costs, providing valuable insights for companies bidding against SpaceX.

This repository contains a Jupyter Notebook with an interactive dashboard built using Plotly Dash. The dashboard visualizes SpaceX launch data, including success rates by launch site and payload mass correlations, to explore factors influencing landing outcomes.

Objectives
Data Visualization: Create an interactive dashboard to explore SpaceX launch data.
Exploratory Analysis: Analyze relationships between launch sites, payload mass, and landing success.
Cost Estimation: Provide insights into launch cost estimation based on landing success.
Dataset
The project uses the spacex_launch_dash.csv dataset, which includes:

Launch Site: The site from which the rocket was launched (e.g., CCAFS LC-40, VAFB SLC-4E).
Payload Mass (kg): The mass of the payload in kilograms.
Class: Binary indicator of landing success (1 = success, 0 = failure).
Booster Version Category: The version of the Falcon 9 booster.
If you don’t have this file, you can:

Download a similar dataset from public sources (e.g., Kaggle: SpaceX Launch Dataset).
Use the dummy dataset provided in the fallback code.
Features
Launch Site Dropdown: Select a specific launch site or view all sites to filter the data.
Success Pie Chart: Displays the proportion of successful landings, either for all sites or a selected site.
Payload Range Slider: Filter data by payload mass to explore its impact on landing success.
Scatter Plot: Visualizes the correlation between payload mass and landing success, colored by booster version.
Requirements
To run this project, install the following Python libraries:

bash

Collapse

Wrap

Copy
pip install dash pandas plotly jupyter-dash
Python: 3.8+
Dash: For building the interactive dashboard.
Pandas: For data manipulation.
Plotly: For creating interactive visualizations.
Jupyter Notebook: For running the code interactively.
Installation
Clone this repository:
bash

Collapse


Wrap

Copy
git clone https://github.com/your-username/spacex-falcon9-landing-prediction.git
cd spacex-falcon9-landing-prediction
Install dependencies:
bash

Collapse

Wrap

Copy
pip install -r requirements.txt
(Create a requirements.txt file with the above libraries if not already present.)
Ensure spacex_launch_dash.csv is in the project directory, or update the file path in the code.
Usage
Open the Jupyter Notebook:
bash

Collapse

Wrap

Copy
jupyter notebook SpaceX_Dashboard.ipynb
Run all cells in the notebook. The dashboard will render inline below the last cell.
Interact with the dashboard:
Use the dropdown to select a launch site.
Adjust the payload slider to filter by mass range.
Observe updates in the pie chart and scatter plot.
Code Structure
SpaceX_Dashboard.ipynb: Main notebook containing the Dash app code.
spacex_launch_dash.csv: Dataset file (required).
requirements.txt: List of dependencies (optional, create if needed).
Example Output
Pie Chart: Shows the success rate for "All Sites" or a specific site (e.g., 70% success for CCAFS LC-40).
Scatter Plot: Plots payload mass vs. landing success, with points sized by mass and colored by booster version.
Troubleshooting
FileNotFoundError: Ensure spacex_launch_dash.csv is in the working directory or update the path in pd.read_csv().
Dash Not Rendering: Verify all dependencies are installed and restart the Jupyter kernel.
Deprecation Warning: The code uses Dash with jupyter_mode="inline" to avoid JupyterDash deprecation issues.
Future Enhancements
Add machine learning models (e.g., Logistic Regression, Decision Trees) to predict landing success.
Incorporate additional data (e.g., weather conditions, booster age).
Deploy the dashboard as a web app using a service like Heroku.
Acknowledgments
Data inspired by SpaceX launch records.
Built with Plotly Dash and Jupyter Notebook.
Part of an exploratory project to understand SpaceX’s reusable rocket technology.
