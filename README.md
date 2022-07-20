# Data Exploration, Cleaning, Visualization and Correlation

## Key Findings

USA was one of the biggest victim of COVID-19 in terms of COVID-19 cases, death counts and was one of the top contries to respond against it with rapid vaccination. New cases were decreased significantly after November 2021 in USA. Total death count was highest in Europe among continents. Vaccinations started in USA on December 2020 and by May 2022, 66.65% people were fully vaccinated. 

## Resources

* Microsoft SQL Server Management Studio
* Google Cloud Services (Cloud SQL)
* Tableau
* Python (Pandas)

## Dataset

Data collected from https://www.worldometers.info/coronavirus/

Modified 1: https://drive.google.com/file/d/1nW08bdKSjJqNtVC53bY07q1X-1Cof4Sg/view?usp=sharing

Modified 2: https://drive.google.com/file/d/1qR1Gt9YQGRzrQzRpeFD7QTunRsfoRMst/view?usp=sharing

## Works done

## Data Exploration SQL 

* Created queries using sub-queries, partitions, join, CTE, temp table, window function etc. 
* Extracted information regarding COVID-19 deaths, cases and vaccinations across the world. 
* Countries affected most in COVID-19 and countries were fast to respond with vaccination. 
* Information in both country and continent wise. 

## Data Visualization in Tableau


<div class='tableauPlaceholder' id='viz1658011746897' style='position: relative'>
<a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;fi&#47;first_16557649026740&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='first_16557649026740&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;fi&#47;first_16557649026740&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>

for interactive dashboard, click <a href="https://public.tableau.com/shared/S689FSFPB?:display_count=n&:origin=viz_share_link">here</a>


<div class='tableauPlaceholder' id='viz1658279229524' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Gl&#47;GlobalVaccinationReport&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='GlobalVaccinationReport&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Gl&#47;GlobalVaccinationReport&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>

for interactive dashboard, click <a href="https://public.tableau.com/views/GlobalVaccinationReport/Dashboard1?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link">here</a>

## 3. Data Cleaning in SQL

* Changed the date format to 'yyy-MM-dd' format.
* Split complete location address to street address, city, state and zip code (substring & parsename). 
* Brought consistency in data (e.g. ('Y', 'Yes') to 'Yes').  
* Handled duplicate rows and remove irrelevant columns. 

Dataset: https://docs.google.com/spreadsheets/d/1c8IQveix6Ly5pPAezQ0xaGoSh3ObXuxC/edit?usp=sharing&ouid=112644935180655994459&rtpof=true&sd=true

## Data Correlation using Python

* Replaced missing values with zero.
* Fixed data type of numerical value columns. 
* Dropped duplicate columns.
* Unstacked data to find highest correlated features in the data. 

Dataset: https://drive.google.com/file/d/1K9RORIgg2pmFeM3OAtv-ShMifi4CQg3x/view?usp=sharing
