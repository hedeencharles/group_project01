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
The correlation coefficient for the In-State and Out-of-State regression lines were **0.940 and 0.936** respectively. Given our regression analysis, we identified a strong positive correlation between both in and out of state tuition costs with number of total applicants.
The slope of the regression line in the In-State and Out-of-State Tuition scatterplots are **0.166 and 0.538** respectively, suggesting a stronger relationship between the variables in the Out-of-State scenario. 

### Question: Are there any differences between in state and out of state tuition cost change over time? 
Over time, tuition has increased for both in and out of state students. We identified this could be for various reasons (inflation, government pressure,etc.). Tuition was overall more expensive for out of state students, while also increasing at a larger rate for out of state. Stanford and USC had unique data and did not follow the samee trend as other schools, as their in and out of state tuitions are equal over time, increasing and decreasing together.

**Washington Region Applications Received vs Tuition In-State and Out-of-State**
![Apps Received OR](/Analysis_Graphs/admiss_vs_apps_graphs/applicants_WA.png)
![TUITION IN-OR](/Analysis_Graphs/state_tuition_graphs/WASHINGTON_IN.png)
![TUITION OUT-OR](/Analysis_Graphs/state_tuition_graphs/WASHINGTON_OUT.png)

**Oregon Region Applications Received vs Tuition In-State and Out-of-State**
![Apps Received OR](/Analysis_Graphs/admiss_vs_apps_graphs/applicants_OR.png)
![TUITION IN-OR](/Analysis_Graphs/state_tuition_graphs/OREGON_IN.png)
![TUITION OUT-OR](/Analysis_Graphs/state_tuition_graphs/OREGON_OUT.png)

**California Region Applications Received vs Tuition In-State and Out-of-State**
![Apps Received OR](/Analysis_Graphs/admiss_vs_apps_graphs/applicants_CA.png)
![TUITION IN-OR](/Analysis_Graphs/state_tuition_graphs/CALIFORNIA_IN.png)
![TUITION OUT-OR](/Analysis_Graphs/state_tuition_graphs/CALIFORNIA_OUT.png)

This furthers our belief that there could be a correlation between in and out of state tuition cost and application numbers, with an emphasis on out of state tuition cost.
Points in time where in and out of state costs differ the most is when the total number of applicants is increasing for some states. Again, we see USC and Stanford presenting a different dynamic and may not be relevant to compare to the other Pac-12 schools.

### Question: Is there a relationship between admissions and applications over time?
Both applications and admissions had an increasing relationship between the years 2002-2018. For most schools we analyzed, we saw a clear relationship between admission numbers and application numbers. We came to conclude this can be for a multitude of reasons; school popularity, career earnings, increased campus size over years, etc. 
A relationship we did identify that is worth noting is, the closer that the admissions curve and applications curve moved together, correlated with higher admissions rate for the particular school. We can very easily see this relationship with Arizona State's curves, as they are nearly identical. Arizona Sate has a very high acceptance rate, recorded as high as 90% acceptance rate. Vice versa, with Stanford we see an increase in number of applications over time, but no change at all in admission numbers. Stanford year after year holds low acceptance rates, which decrease as number of applicants increases (logically).

**Washington Region Applications Received vs Students Admitted**
![Apps Received WA](/Analysis_Graphs/admiss_vs_apps_graphs/applicants_WA.png)
![Admission WA](/Analysis_Graphs/admiss_vs_apps_graphs/admissions_WA.png)

**Arizona Region Applications Received vs Students Admitted**
![Apps Received AZ](/Analysis_Graphs/admiss_vs_apps_graphs/applicants_AZ.png)
![Admission AZ](/Analysis_Graphs/admiss_vs_apps_graphs/admissions_AZ.png)

**California Region Applications Received vs Students Admitted**
![Apps Received WA](/Analysis_Graphs/admiss_vs_apps_graphs/applicants_CA.png) ![Admission WA](/Analysis_Graphs/admiss_vs_apps_graphs/admissions_CA.png)

Given the schools we analyzed, we observed similar trends in all schools accept for Stanford and USC, whos two schools are a different dynamic. If we were to run our analysis again, we would take out Stanford and USC as they are clear outliers and most likely skewed our calculations. Overall, we did observe a positive relationship between application numbers and tuition, as well as a relationship with admissions numbers and number of applicants.
