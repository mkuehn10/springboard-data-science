# Capstone Project Proposal

## What is the problem you want to solve?
A recent article ["WV graduation rates don't show if students are ready for college"](https://www.wvgazettemail.com/news/education/wv-graduation-rates-don-t-show-if-students-are-ready/article_407a3615-45c7-5330-8c98-a2cea1a18da9.html), discussed how schools in West Virginia are being lauded for their graduation rates.  The problem is that this isn't necessarily carrying over to the college-level.  Does a higher graduation rate really mean a school is doing a better job?  Do high standardized test scores indicate excellence?  What are the indicators that students, teachers, schools, administrators, and boards of education are doing a good job?

## Who is your client and why do they care about this problem? In other words, what will your client DO or DECIDE based on your analysis that they wouldn’t have otherwise?
My client is anyone with a vested interest in public education.  The primary audience for this project would be school- and district-level administrators.  This project will provide information about which indicators are important in evaluating student performance.

## What data are you going to use for this? How will you acquire this data?
The West Virginia Department of Education provides data on their [ZOOM WV Data Dashboard](https://zoomwv.k12.wv.us/Dashboard/portalHome.jsp).  The following information is available:

* School Composition (Enrollment & Demographic)
* Graduation Rate by County & Demographic
* Assessment Proficiency Summary by School, County, & Demographic
* Attendance Rate by County & Demographic
* Dropout Rate by County & Demographic
* Percent of Students that are considered Needy by County & School
* Miles Traveled and Passengers Transported by County
* Historical Promotion/Retention Data by County & Grade
* Percent of Courses Taught by Highly Qualified Teachers by County

## In brief, outline your approach to solving this problem (knowing that this might change later).
1) **Gather, clean, and merge the data**: The data from the ZOOM WV Data Dashboard is available in separate files.  Some of the files are broken down by individual school, and some are by county.  Some data is only available from prior years.  Care will need to be taken to make assumptions and justify the use of this data.  Any available data at the school level will be recorded in a school data table.  Any other data will be aggregated and will be recorded in a county data table.

2) **Exploratory Data Analysis**: The data will be examined at a high-level to notice any trends or interesting observations.  Data will be viewed by subgroups such as county, gender, ethnicity, and special education to see if there are any differences between groups.  The assessment scores and graduation rates will be looked at with the ultimate goal that they could possibly be target variables for prediction purposes.

3) **Cluster Analysis**: The features for each county and school will be used to examine any clustering.  This will be useful in attempting to make recommendations to policy (schools that are similar based on the available data may benefit from the same changes to policy).  Recommendations for policy changes may also be different for different clusters of schools.

4) **Feature Selection for Predicting Graduation Rates/Assessment Scores**: Predictive models will be created to attempt to find the most important features that have an effect on graduation rates and assessment scores for the purpose of providing guidance to administrators on which factors may be worthwhile to focus on (e.g. attendance versus highly qualified teachers).

## What are your deliverables? Typically, this would include code, along with a paper and/or a slide deck.
The deliverables for this project will be several Jupyter notebooks with the code corresponding to the different phases of the project described above.  A paper describing the entire data analysis process will be created.  A slide presentation with a summary of findings and interesting observations will also be included.