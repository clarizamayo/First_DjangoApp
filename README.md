### Your tasks for this lab:

1. Create a jupyter notebook stored in `/notebooks` for your initial work. In it, start to document your process. Include some of the following:
* the topic you would like to focus on
* some initial data you found that could work for your analysis
* initial exploratory data analysis to see if data gathered is viable
* outside information that could be useful to your process (charts, articles, links that are relevant to your topic.
2. Find some initial data pertaining to your topic and store the files in the `/data` folder.
3. If you would like to scrape data, find some source that could potentially be scraped and begin inspecting it for ways to obtain it. It might be beneficial to do this in a jupyter notebook initially and then once you have some working code, place it into a `*.py` file in `/scripts`.
4. Create a `README.md` file containing information about your project. Keep it simple. We'll continue to add to this over time. 
5. An initial view in your django application (we'll learn templating next week but feel free to work ahead)

Minimum requirements for lab grade are:
* a github link to your repo with commits
* a `*.ipynb` file in `/notebooks` with your initial work (see above bulletpoints)
* a potential or relevant dataset in `/data`
* a `README.md` file

Commit your changes to the your repo at the end of class time and submit a link to google classroom. You have until Sunday to add further commits.

## I will be pulling information from the kaggle api:
https://www.kaggle.com/uciml/student-alcohol-consumption

### 3 files:
- student-mat.csv

- student-merge.R

- student-por.csv

For now I will explore them in this notebook and then create the scripts.py and the import.py to my app.

## Content:
**Attributes for both student-mat.csv (Math course) and student-por.csv (Portuguese language course) datasets:**

- school - student's school (binary: 'GP' - Gabriel Pereira or 'MS' - Mousinho da Silveira)
- sex - student's sex (binary: 'F' - female or 'M' - male)
- age - student's age (numeric: from 15 to 22)
- address - student's home address type (binary: 'U' - urban or 'R' - rural)
- famsize - family size (binary: 'LE3' - less or equal to 3 or 'GT3' - greater than 3)
- Pstatus - parent's cohabitation status (binary: 'T' - living together or 'A' - apart)
- Medu - mother's education (numeric: 0 - none, 1 - primary education (4th grade), 2 – 5th to - 9th grade, 3 – secondary education or 4 – higher education)
- Fedu - father's education (numeric: 0 - none, 1 - primary education (4th grade), 2 – 5th to - 9th grade, 3 – secondary education or 4 – higher education)
- Mjob - mother's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'at_home' or 'other')
- Fjob - father's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'at_home' or 'other')
- reason - reason to choose this school (nominal: close to 'home', school 'reputation', 'course' preference or 'other')
- guardian - student's guardian (nominal: 'mother', 'father' or 'other')
- traveltime - home to school travel time (numeric: 1 - 1 hour)
- studytime - weekly study time (numeric: 1 - 10 hours)
- failures - number of past class failures (numeric: n if 1<=n<3, else 4)
- schoolsup - extra educational support (binary: yes or no)
- famsup - family educational support (binary: yes or no)
- paid - extra paid classes within the course subject (Math or Portuguese) (binary: yes or no)
- activities - extra-curricular activities (binary: yes or no)
- nursery - attended nursery school (binary: yes or no)
- higher - wants to take higher education (binary: yes or no)
- internet - Internet access at home (binary: yes or no)
- romantic - with a romantic relationship (binary: yes or no)
- famrel - quality of family relationships (numeric: from 1 - very bad to 5 - excellent)
- freetime - free time after school (numeric: from 1 - very low to 5 - very high)
- goout - going out with friends (numeric: from 1 - very low to 5 - very high)
- Dalc - workday alcohol consumption (numeric: from 1 - very low to 5 - very high)
- Walc - weekend alcohol consumption (numeric: from 1 - very low to 5 - very high)
- health - current health status (numeric: from 1 - very bad to 5 - very good)
- absences - number of school absences (numeric: from 0 to 93)
- These grades are related with the course subject, Math or Portuguese:

- G1 - first period grade (numeric: from 0 to 20)
- G2 - second period grade (numeric: from 0 to 20)
- G3 - final grade (numeric: from 0 to 20, output target)

**Additional note: there are several (382) students that belong to both datasets .
These students can be identified by searching for identical attributes
that characterize each student, as shown in the annexed R file.**
