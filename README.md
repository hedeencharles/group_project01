# Charles_branch Read.me
Project 01 - Group 2
====================

=========================================================================

Project write-up:
=================

- Write this as a brief summary of your interests and intent, including:

Uncover trends that affect enrollment, tuition and admissions:
    We will be adressing the relationships and trends in data regarding the number of college applications (compare instate and out of state), and change in acceptance rate over time (we plan to determine given what data we find). We will be using percent change over time for acceptance rate in order to keep the analysis relative between schools. We will also compare in state vs out of state applications and percent change over tiem. We will better be able to define the parameters of our project as we mine data, but as of now we know we know we will be scoping in on:
    - Parameters:
    1) Specific time frame (ex. 1980-2010)
    2) Narrowing the schools down to a specific region (or school conference) of the united states. 
    3) Using percent changes to keep numbers relative
    4) Only use "first-time applicants" in data
    
    
- The kind of data you'd like to work with/field you're interested in (e.g., geodata, weather data, etc.)

    - Each college's percent accetpance rate data and change in acceptance rate over specified time frame.
    - Each college's percent acceptance rate data and change in acceptance rate over specified time frame.
    - In state vs out of state applicants
    - Data from specific region of the US or specific college conference 

- The kinds of questions you'll be asking of that data
    - Trends/spikes in admissions acceptance rate over specified time
    - Are colleges recieving more instate or out of state applicants and the percent change overtime.

- Possible source for such data
    https://collegescorecard.ed.gov/data/documentation/ ,
    https://collegeai.com/data/ ,
    https://educationdata.urban.org/documentation/#how_to_use 

- Work flow breakdown
    - Charles and Pheobe: 
        - Are going to work with the API and pull the data we need (tuition cost, acceptance rate and number of instate/out of state applicants). Are responsible for setting up data to then be broken into dataframes for further cleaning and analysis.
    - Nick and Erin
        - Are going to keep looking for relevant data and forming the questions further until Charlie and Pheobe complete work requesting the API. Nick and Erin will then work together to create DataFrames for analysis.
    - Once DataFrames are creating, run calculations, run regressions, make graphs, etc. 


Final write-up summary:
=================

### Charles Hedeen, Erin Hislope, Nick Ameroso, and Phoebe Rosoff
## PAC-12 Tuition Changes: 2002-2018

### Question: Is there a relationship between number of applications received per year and tuition for that year?

**Regression Analysis Scatterplot for all Pac-12 Universities Applications vs In-State and Out-of State Tuition Cost**
![Regression Scatterplot IN](/Analysis_Graphs/regressions_graphs/TTL_apps_vs_tuition_IN.png)
![Regression Scatterplot OUT](/Analysis_Graphs/regressions_graphs/TTL_apps_vs_tuition_OUT.png)

When analyzing data on number of applicants and tuition costs we found a relationship between the two.
The correlation coefficient for the In-State and Out-of-State regression lines were **0.940 and 0.936** respectively. Given our regression analysis, we identified a positive correlation between both in and out of state tuition costs with number of applicants.
The slope of the regression line in the In-State and Out-of-State Tuition scatterplots are **0.166 and 0.538** respectively, suggesting a possibly stronger relationship between the variables in the Out-of-State scenario.

### Question: Are there any differences between in state and out of state tuition cost change over time? 
Over time, tuition has increased for both in and out of state students, while increasing at a greater rate for out of state.
Points in time where in and out of state costs differ the most is when the total number of applicants is increasing for some states. 

**Oregon Region Applications Received vs Tuition In-State and Out-of-State**
![Apps Received OR](/Analysis_Graphs/admiss_vs_apps_graphs/applicants_OR.png)
![TUITION IN-OR](/Analysis_Graphs/state_tuition_graphs/OREGON_IN.png)
![TUITION OUT-OR](/Analysis_Graphs/state_tuition_graphs/OREGON_OUT.png)
This furthers our belief that there could be a correlation between in and out of state tuition cost and application numbers, with an emphasis on out of state tuition cost.

### Question: Is there a relationship between admissions and applications over time?
Both applications and admissions had an increasing trend over the time frame studied. For the most part, spikes and dips in the numbers of applications translated to similar patterns in admissions values.

**Washington Region Applications Received vs Students Admitted**
![Apps Received WA](/Analysis_Graphs/admiss_vs_apps_graphs/applicants_WA.png)
![Admission WA](/Analysis_Graphs/admiss_vs_apps_graphs/admissions_WA.png)

**Arizona Region Applications Received vs Students Admitted**
![Apps Received AZ](/Analysis_Graphs/admiss_vs_apps_graphs/applicants_AZ.png)
![Admission AZ](/Analysis_Graphs/admiss_vs_apps_graphs/admissions_AZ.png)
There were some data that did not follow this pattern as closely, namely the California schools. While we realize there are many factors that may affect a University's capacity to accept students at any given year, in most regions the admission rates seem to follow similar patterns that the application rates do in their respective regions.
