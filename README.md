# SD_data_contest_education_3-10
2015 San Diego Data Analysis Contest

What is the demographic profile of the typical ELA student?
<ul>
    <li>machine learning/regression analysis</li>
</ul>
What are the most important correlations of CELDT and with demographic factors. 
<ul>
    <li>correlations</li>
</ul>
What are the strongest predictors of performance on the CELDT and ELA  test?
<ul>
    <li>machine learning (predictive model)</li>
</ul>
Which schools perform better  on the CST ELA than would be predicted by their demographic factors.  Break out the performance of RFEP ( Reclassified as English Fluent Proficient ) students, if possible. 
<ul>
    <li>We need to answer the previous question first</li>
</ul>
Do schools with a high or low density of ELL students have better or worse performance than you would predict?
<ul>
    <li>We need to answer the previous question first</li>
</ul>
Present any interesting or notable patterns. 
Are some schools better than others at preparing formerly ELL students to do well in school after they have been reclassified as proficient?
<ul>
    <li>Is there a way to track specific students?</li>
</ul>


1. Do language learners of some languages have an easier or more difficult time learning English than native speakers of other languages? (eg. do Spanish speakers learn English quicker than say speakers of Kurdish)?
 * We can look at CELDT tests across primary language
2. Can we see if families utilize other social services available (tutoring, food assistance, community groups, etc.), and if so, does this type of community involvement have an effect on English learning ability?
 * We can look at the number of students getting school lunches and the EL tests
 
 ---------------------------------------
 How to marry the files
 
 All files have a cds_code column, with each school being associated with the same code across all files.
 
  Each row needs to be one school with all of the data associated with that school.
  To create only one row for each school we need to transform data files by taking multiple rows and making them one. In order to do this and still track the necessary components we need to take each of the columns (listed below for each specific document), code the column into the rest of the column names, and then combine the columns. We should probably talk about this over the phone.
 
 
 use:
 api_2012
 
 celdt
  - subgroup ID  00
  - overall performance level  0
  - test purpose  0
  - grade  00
  000000_columnName
  
star
 - subgroup  000
 - grade  00
 - test_id  00
 0000000_columnName
 
enroll_2013
 - ethnic  0
 - gender L
 0L_columnName
