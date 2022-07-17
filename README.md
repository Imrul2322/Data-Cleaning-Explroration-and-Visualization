# Data Exploration, Cleaning, Visualization and Correlation

## Key Findings

USA was one of the biggest victim of COVID-19 in terms of COVID-19 cases and death counts. Everage new cases decreased significantly after November 2021 in USA. Total death count was highest in Europe among continents. 

## Environment

1. Microsoft SQL Server Management Studio
2. Google Cloud Services (Cloud SQL)

## Dataset

Data collected from https://www.worldometers.info/coronavirus/

Modified 1: https://drive.google.com/file/d/1nW08bdKSjJqNtVC53bY07q1X-1Cof4Sg/view?usp=sharing
Modified 2: https://drive.google.com/file/d/1qR1Gt9YQGRzrQzRpeFD7QTunRsfoRMst/view?usp=sharing

## Works done

## Data Exploration SQL 

Created queries to extract specific information using sub-queries, partitions, join, CTE, temp table, window function etc. 


Original dataset has a wide range of information related to COVID-19. Information about new cases, new death, new hospitalized count, total count for each cases and many more. I have shown many useful information like death_rate for each country and each continent, extracted date on which each country had highest death count, vaccination rate for each country and many more. Lastly I created view for most important information for using in Tableau. 

## Data Visualization in Tableau
Then I created Tableau dashboard showing useful information I extracted using SQL queries in first part. In one dashboard I have shown covid-19 death related information. Total death count with death rate overall, new covid-19 cases where I have shown that, from December 2021, new covid-19 cases have been decreased drastically because of rapid and mass vaccination. I have shown 6 specific counties information including US. Next, I have implemented death count information in a geographic manner using openstreetmap. And lastly, there is death count by continent. Of course there is lot to learn but it's just a matter of time. 


<div class='tableauPlaceholder' id='viz1658011746897' style='position: relative'>
<a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;fi&#47;first_16557649026740&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='first_16557649026740&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;fi&#47;first_16557649026740&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>

for interactive dashboard, click <a href="https://public.tableau.com/shared/S689FSFPB?:display_count=n&:origin=viz_share_link">here</a>

## 3. Data Cleaning in SQL
I took a glance on the whole dataset at first and found several things to work on. I changed the format of dates which are not standard to standard one 'yyy-MM-dd'. Then, addresses had street address, city and state together. I used both substring and parsename to seperate them into three different columns. Some columns had inconsistent data like instead of 'No', some places it was just 'N' or 'False', I change them to a standard 'No'. Then I dealt with duplicate rows and renoves unnecessary columns. 

Origial Dataset: https://docs.google.com/spreadsheets/d/1c8IQveix6Ly5pPAezQ0xaGoSh3ObXuxC/edit?usp=sharing&ouid=112644935180655994459&rtpof=true&sd=true

## Data Correlation using Python

In this section, I worked with pandas dataframe to find correlation of features in the dataset. At first, I dealt with the missing values which I replaced with 0. I could replace with other values like mode, median, mean depending on the data. Then, I changed the datatypes of some columns which had numeric values but it was read as object columns. Dropped the duplicate ones. Then, I plotted regression among features to find correlation. I created the correlation matrix and showed in a headmap. My goal was to find the highest correlated features in the dataset. I converted all the dataframe columns which were not neumeric and then find the correlation matrix. Next, I unstacked the data and sorted to find the highest correlated features in a table with correlation values. Finally, found three most correlated features. 

Original Dataset: https://drive.google.com/file/d/1K9RORIgg2pmFeM3OAtv-ShMifi4CQg3x/view?usp=sharing
