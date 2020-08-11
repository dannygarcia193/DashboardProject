# DASHBOARD AUTOMATION PROJECT

## DESCRIPTION
This is submission to Practicum by Yandex's Dashboard Automation Project.

Based on technical requirements as provided by the Practicum, the
dashboard serves to answer three common questions relating to YouTube trending videos:
   (1) What video categories were trending last week?
   (2) How were they distributed among various regions?
   (3) What categories were especially popular in the United States?

Hypothetically speaking, the insights from the dashboard will help marketing managers make data-driven decisions regarding the
types of content demanding marketing attention.
## CONTENTS
requirements.txt:
Lists the python libraries and their respective version that are required to run the project

pipelineScript.ipynb:
Jupyter notebook script that connects to database, retrieves, and then downloads the database table (trending_by_time) to use for Tableau dashboard.

trending_by_time.csv:
Data on trending Youtube videos in select regions containing the following relevant columns: region (country/geographical region),
trending_date (date and time), category_title (video category),videos_count (number of videos in the trending section)

DashboardProject.pptx:
Presentation on analyses and recommendation for content that deserves marketing attention based
off trending videos on Youtube.

[https://public.tableau.com/views/DashboardProject_15969044432290/TrendingYoutubeVidz?:language=en&:display_count=y&publish=yes&:origin=viz_share_link](Link) to dashboard on Tableau Public's server:


## HOW TO USE
(1) Download and install Tableau Public ([https://public.tableau.com/en-us/s/download](free)) or Desktop ([https://www.tableau.com/products/desktop/download](paid)).

(2) Access and download Tableau workbook (see link to dashboard on Tableau Public's server) for the calculations, dimensions, etc. used to create the
dashboard.

(3) Install required libraries, if needed. Library requirements can be installed using pip installer:

    pip install -r requirements.txt

(4) Run the script using the Jupyter Notebook provided in this folder (pipelineScript.ipynb). This
will save an updated version of the csv dataset (trending_by_time.csv) in the current working directory.

(4) Run the downloaded workbook from step 2. Make sure that the most recent version of
the dataset trending_by_time.csv is connected as the data source.

(5) To keep the dashboard with the most up-to-date data, click on the following in Tableau: Data-> Data Source -> "Refresh Data Source" or "Refresh All Extracts ..."

Dataset is updated midnight UTC. Run pipeline script and refresh data source as needed to keep dashboard up to date.
