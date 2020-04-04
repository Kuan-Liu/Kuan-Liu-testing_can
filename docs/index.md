---
title: "COVID-19 Testing Data and Trend in Canada"
knit: (function(input_file, encoding) {
  out_dir <- 'docs';
  rmarkdown::render(input_file,
 encoding=encoding,
 output_file=file.path(dirname(input_file), out_dir, 'index.html'))})
author: 
- "Kuan Liu, kuan.liu@mail.utoronto.ca"
- "Alexandra Bushby, alex.bushby@mail.utoronto.ca"
- "Thai-Son Tang, thaison.tang@mail.utoronto.ca"

output:
  html_document:
    keep_md: true
    highlight: haddock
    number_sections: false
    self_contained: yes
    toc: yes
    toc_depth: 3
    toc_float: yes
---

**Date Created:** Mar 25, 2020

**Date Updated:** Apr 04, 2020 3:10:50 PM EDT

**Code Avaliable at** https://github.com/Kuan-Liu/Kuan-Liu-testing_can




**From the authors: Thank you for your interest in our work! We are constantly working to improve this website and all comments and feedbacks are welcome. For most accurate and reliable Canadian COVID-19 epidemiology data, please visit Public Health Agency of Canada COVID-19 report site at https://www.canada.ca/en/public-health/services/diseases/2019-novel-coronavirus-infection.html (Full PDF report available).**

## Acknowledgment
Data used in this repostory are extracted from the data speardsheet posted by the COVID-19 Canada Open Data Working Group (https://github.com/ishaberry/Covid19Canada). This working group, lead by Isha Berry and Jean-Paul R. Soucy from Dalla Lana School of Public Health, Unviersity of Toronto, has created an interactive dashboard on Canadian COVID-19 epidemiology data. We direct readers to visit the dashboard at https://art-bd.shinyapps.io/covid19canada/.

## 1. Objectives and key messages
 - Providing information on testing capacity and trend overtime in Canada to **identify gaps and needs to increase testing capacity**.
 - Providing information on testing results, sepcifcially the proporion of patients reported positive, to **provide inslight on testing protocols**. When testing resources are limited, protocols to grant testing are likely to be modified to maximize health outcomes. For instance, symptomatic patients in high risk group for severe outcomes are given testing priority.

## 2. Total number of tests to date

<!-- ### 2.1 Nation-wide total number of tests to date -->

<!-- As of March 30, 2020 (6 pm EDT), the total number of patients tested in Canada is **184,201** and the total number of patients tested per 100,000 population in Canada is around **490**. -->

<!--   - the total number of patients tested positive is **5,153 (2.8%)** -->
<!--   - the total number of patients tested negative is **166,621 (90.5%)** -->
<!--   - the rest **12,427 (6.7%)** patients are likely under investigation waiting for test results, detailed information is not available. -->

### 2.1 Total number of tests to date by province and territory

- **Highlights**
  - **Alberta, Quebec and British Columbia are the top three provinces ranking by the number of tests per 100,000 population.**
  - **Quebec has rapidly increased its testing capacity. The total number of tests per 100,000 population has increased to 1035 as of Apr 3, 2020, comparing to 365 on Mar 25, 2020.**
  - **Northwest territories and Yukon reported over 1500 tests per 100,000 population, highest in Canada.**

<img src="C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-1-1.png" style="display: block; margin: auto;" />


Table: Reported testing data province and territory, public data accessed online as of  Apr 04, 2020 3:10:53 PM

 Province    Reported Positive    Reported Negative    Reported Pending    Total    Est. Population    Total per 100,000 population 
----------  -------------------  -------------------  ------------------  -------  -----------------  ------------------------------
    AB             1075                   -                   -            61960        4371316                    1417             
    QC             6101                 77469                4233          87803        8484965                    1035             
    SK              220                   -                   -            11720        1174462                    998              
    BC             1174                   -                   -            47352        5071336                    934              
    MB              182                   -                   -            11952        1369465                    873              
    NS              207                 8234                  -            8441         971395                     869              
    PE              22                   813                 264           1099         156947                     700              
    NL              195                   -                   -            3201         521542                     614              
    NB              95                  4661                  -            4756         776827                     612              
    ON             3255                 62253                1245          66753       14566547                    458              



 Territory    Reported Positive    Reported Negative    Reported Pending    Total    Est. Population    Total per 100,000 population 
-----------  -------------------  -------------------  ------------------  -------  -----------------  ------------------------------
    NT                4                  1137                 117           1258          44826                     2806             
    YT                6                   694                  53            753          40854                     1843             
    NU                0                   98                  216            314          38780                     810              

###### Footnote: It's likely individuals may have been tested more than once. We are collecting publicly avaliable information online to best match patients with testing numbers. Unfortunately, detailed information is not always avaiable, so please read these data with caution. Reported positive tests include resolved and deceased cases.


### 2.2 Relation between cases and tests

#### Geographic mapping on the total number of tests, total number of cases, total number of tests per 100,000 population and total number of cases per 100,000 population as of Apr 04, 2020 3:10:53 PM
<img src="C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-3-1.png" style="display: block; margin: auto;" />

### 2.3 Estimated Test-Case Ratio
We define the test-case ratio (TCR) as
$$
TCR= \frac{\text{Total number of postive cases}}{\text{Total number of tests completed}},
$$
which is also known as the proportion of positives cases. For provinces and territories that reported total number of tests including under investigation tests. The demoninator has be asjusted to inclunde only the completed, results known tests.

**Interpretation: Provinces and territories above the national line demonstrate higher proportion of tested inidividuals being postive - individuals tested in these areas are relatively more likely to be positive; Similarly, provinces and territories below the national line demonstrate lower proportion of tested individuals being positive - individuals tested in these areas are relatively less likely to be positive.**

<img src="C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-4-1.png" style="display: block; margin: auto;" />

## 3. Cumulative tests overtime

- **Highlights**
  - **Consistent increase of testing capacity overtime across Canada.**   
  - **Quebec displays a sharp testing increase on March 25, 2020. British Columbia displays a shart testing increase on March 20, 2020.**
  - **Alberta, Ontario, British Columbia and Quebec are the top 4 provinces ranked by the total number of cumulative tests with Quebec as the leading province**
  - **It seems Ontario is falling slight behind on the testing capacity per capita. **

<img src="C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-5-1.gif" style="display: block; margin: auto;" />

<img src="C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-6-1.png" style="display: block; margin: auto;" /><img src="C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-6-2.png" style="display: block; margin: auto;" />

<img src="C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-7-1.png" style="display: block; margin: auto;" />



## 4. Tests completed per day 

- **Highlights**
  - **Quebec has increased its testing capacity on March 22, 2020 to allow the direct inclusion of hospital laboratories' testing results. This explains the observed dramatic increase on the number of tests completed on March 24, 2020. It's likely these additional tests reported on that day were completed over the past two days.**
  - **The number of tests completed per day does NOT directly reflect regional testing capacity. Provinces and territories with small number of COVID-19 cases are expected to complete less tests per day.**


**Methods.** The number of tests completed per day is estimated by taking the difference between the cumulative number of tests on two consequtive days within each region. On days when no cumulative tests were reported, we carried forward the last observed value and treated all zero values of the consequtive cumulative tests' difference as missing. For example, 

The number of tests completed on March 25 in Ontario 

= the number of tests cumulative tests reported on March 26 in Ontario - the number of tests cumulative tests reported on March 25 in Ontario = 38550 - 	35635 = 2915.

On March 30, 2020 Ontario changed reporting thus causing the daily test estimate to be negative. We flagged it as missing (no point on the Ontario green curve on March 29th), when producing the below daily test plot.

<!-- made error reported alberta instead of ontario -->
<img src="C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-8-1.png" style="display: block; margin: auto;" /><img src="C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-8-2.png" style="display: block; margin: auto;" />

## 5. Testing results to date

- **Highlights**
  - **Nunavut has no confirmed case yet.**
  - **Quebec has the highest proportion of positive tests (6.9%).**
  - **There appears to be a back log of test reporting in Prince Edward Island and Nunvaut. The back log in Ontario is observed to be cleared. The proportion of pending tests in Ontario has reduced significantly, at 1.9% now comparing to the same proportion on Mar 25, 2020 at 29.4%.**
  
<img src="C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-9-1.png" style="display: block; margin: auto;" />


###### Footnote: For provinces that don't report pending cases, we will assume a binary testing status (postive or negative).

  
<!-- ### Important jurisdiction-specific dates -->

<!--   - March 22, 2020, Nova Scotia declared state of emergency -->
<!--   - March 20, 2020, Manitoba declares state of emergency -->
<!--   - March 20, 2020, Northwest Territories declared public health emergency -->
<!--   - March 19, 2020, New Brunswick declared state of emergency -->
<!--   - March 18, 2020, Newfoundland and Labrador declared public health emergency -->
<!--   - March 18, 2020, Yukon declared public health emergency -->
<!--   - March 18, 2020, Saskatchewan declared state of emergency -->
<!--   - March 18, 2020, British Columbia declared provintial state of emergency -->
<!--   - March 17, 2020, Nunavat declared public health emergency -->
<!--   - March 17, 2020, Alberta declared state of emergency -->
<!--   - March 17, 2020, Ontario declared state of emergency -->
<!--   - March 16, 2020, Prince Edward Island declared public health emergency -->
<!--   - March 13, 2020, Quebec declared health emergency -->


## Reference

- COVID-19 Canada Open Data Working Group. Epidemiological Data from the COVID-19 Outbreak in Canada. https://github.com/ishaberry/Covid19Canada. (2020-03-25).
- [National testing data to date] https://www.canada.ca/en/public-health/services/diseases/2019-novel-coronavirus-infection.html and https://www.ctvnews.ca/health/coronavirus/tracking-every-case-of-covid-19-in-canada-1.4852102
- [Ontario testing data to date] https://www.ontario.ca/page/2019-novel-coronavirus
- [British Columbia testing data to date] http://www.bccdc.ca/about/news-stories/stories/2020/information-on-novel-coronavirus
- [Alberta testing data to date] https://www.alberta.ca/covid-19-alberta-data.aspx
- [Saskatchewan testing data to date] https://www.saskatchewan.ca/government/health-care-administration-and-provider-resources/treatment-procedures-and-guidelines/emerging-public-health-issues/2019-novel-coronavirus/cases-and-risk-of-covid-19-in-saskatchewan()
- [Manitoba testing data to date] https://www.gov.mb.ca/covid19/
- [Quebec testing data to date] https://msss.gouv.qc.ca/professionnels/maladies-infectieuses/coronavirus-2019-ncov/
- [Newfoundland and Labrador testing data to date] https://www.gov.nl.ca/covid-19/
- [New Brunswick testing data to date] https://www2.gnb.ca/content/gnb/en/departments/ocmoh/cdc/content/respiratory_diseases/coronavirus.html
- [Nova Scotia testing data to date] https://novascotia.ca/coronavirus/#cases
- [Prince Edward Island testing data to date] https://www.princeedwardisland.ca/en/topic/covid-19
- [Yukon testing data to date] https://yukon.ca/en/health-and-wellness/health-concerns-diseases-and-conditions/covid-19-information
- [Northwest Territory testing data to date] https://www.hss.gov.nt.ca/en/services/coronavirus-disease-covid-19
- [Nunavut testing data to date] https://www.gov.nu.ca/health/information/covid-19-novel-coronavirus
