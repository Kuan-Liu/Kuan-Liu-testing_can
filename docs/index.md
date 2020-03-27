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

output:
  html_document:
    keep_md: true
    highlight: haddock
    number_sections: no
    self_contained: yes
---

**Date Created:** 2020-03-25

**Date Updated:** 2020-03-27

**Code Avaliable at** https://github.com/Kuan-Liu/Kuan-Liu-testing_can



## Acknowledgement
Data used in this repostory are extracted from the data speardsheet posted by the COVID-19 Canada Open Data Working Group (https://github.com/ishaberry/Covid19Canada). This working group, lead by Isha Berry and Jean-Paul R. Soucy from Dalla Lana School of Public Health, Unviersity of Toronto, has created an interactive dashboard on Canadian COVID-19 epidemiology data. I direct readers to visit the dashboard site at https://art-bd.shinyapps.io/covid19canada/.



## Nation-wide total number of tests to date

As of March 26, 2020 (6 pm EDT), the total number of patients tested in Canada is 161,603 and the total number of patients tested per 10,000 population in Canada is around 42.

  - the total number of patients tested positive is 3,866 (2.39%)
  - the total number of patients tested negative is 145,067 (89.77%)
  - the rest 12,706 patients (7.86%) are likely under investigation waiting for test results, detailed information is not available.

(Data source: https://www.canada.ca/en/public-health/services/diseases/2019-novel-coronavirus-infection.html). 

## Total number of tests to date province and territory

- **Highlights**
  - **Alberta, British Columbia and Saskatchewan are the top three provinces ranking by the number of tests per 10,000 population.**
  - **Northwest territories and Yukon reported over 100 tests per 10,000 population, highest in Canada.**
  - **Only 3 provinces, Ontario, Quebec and Prince Edward Island, reported the number of tests pending results. There appears to be a back log of test reporting in Ontario.**
  

Table: Reported testing data province and territory, public data accessed online as of March 26, 2020 (8 pm EDT). Reported positive tests include resolved and deceased cases.

Province    Reported Positive   Reported Negative   Reported Pending   Total   Est. Population   Total per 10,000 people
---------  ------------------  ------------------  -----------------  ------  ----------------  ------------------------
AB                        486               36174                  -   36660           4371316                        84
BC                        725                   -                  -   31739           5071336                        63
MB                         36                   -                  -    5606           1369465                        41
NB                         33                1795                  -    1828            776827                        24
NL                         82                1409                  -    1491            521542                        29
NS                         73                3201                  -    3274            971395                        34
ON                        858               26727              10965   38550          14566547                        26
PEI                         5                 339                212     556            156947                        35
QC                       1629               31854               2622   36105           8484965                        43
SK                         95                   -                  -    6915           1174462                        59
NWT                         1                 263                295     559             44826                       125
NU                          0                  50                116     166             38780                        43
YT                          3                 412                102     517             40854                       127

  
- **Highlights**
  - **Nunavut has no confirmed case yet.**
  - **Among the 3 provinces that reported pending tests (Quebec, Ontario and Prince Edward Island), Quebec has the highest proportion of positive tests (4.5%).**
  - **Among the 4 provinces that reported negative tests but not tests awaiting for results (Alberta, New Brunswick, Newfoundland and Labrador and Nova Scotia), Newfoundland and Labrador has the highest proportion of positive tests (5.5%). This can be interpreted as for every 100 tests completed (with known results) in Newfoundland and Labrador, we expect around 5 to 6 of them to be postive.**
  
![](C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-2-1.png)<!-- -->

##### Footnote: For provinces that don't report pending cases, we will assume a binary testing status (postive or negative).

## Cumulative tests by province between March 15 - March 26, 2020

- **Highlights**
  - **Consistent increase of testing capacity over the 12-day window across Canada. Quebec displays a sharp testing increase on March 25, 2020. British Columbia displays a shart testing increase on March 20, 2020.**
  - **Alberta, Ontario, British Columbia and Quebec are the top 4 provinces ranked by the total number of cumulative tests**
  - **Alberta, British Columbia and Quebec also rank high among the 10 provinces by the total number of tests conducted per 10,000 population. It seems Ontario is falling slight behind the above three provinces on the testing capacity per capita. **
  - **Despite having low numbers of cumulative tests, the three territories demonstrate above national average testing capacity per capita.**
  
![](C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-3-1.png)<!-- -->

![](C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-4-1.png)<!-- -->


## Cumulative tests by territory

![](C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-5-1.png)<!-- -->

![](C:\Users\KUANLI~1\DROPBO~1\STAT_C~1\BAYESI~1\KUAN-L~1\KUAN-L~1\docs\INDEX_~1/figure-html/unnamed-chunk-6-1.png)<!-- -->


## Important jurisdiction-specific dates

  - March 22, 2020, Nova Scotia declared state of emergency
  - March 20, 2020, Manitoba declares state of emergency
  - March 20, 2020, Northwest Territories declared public health emergency
  - March 19, 2020, New Brunswick declared state of emergency
  - March 18, 2020, Newfoundland and Labrador declared public health emergency
  - March 18, 2020, Yukon declared public health emergency
  - March 18, 2020, Saskatchewan declared state of emergency
  - March 18, 2020, British Columbia declared provintial state of emergency
  - March 17, 2020, Nunavat declared public health emergency
  - March 17, 2020, Alberta declared state of emergency
  - March 17, 2020, Ontario declared state of emergency
  - March 16, 2020, Prince Edward Island declared public health emergency
  - March 13, 2020, Quebec declared health emergency
  

# Reference

- COVID-19 Canada Open Data Working Group. Epidemiological Data from the COVID-19 Outbreak in Canada. https://github.com/ishaberry/Covid19Canada. (2020-03-25).
- [National testing data to date] https://www.canada.ca/en/public-health/services/diseases/2019-novel-coronavirus-infection.html and https://www.ctvnews.ca/health/coronavirus/tracking-every-case-of-covid-19-in-canada-1.4852102
- [Ontario testing data to date] https://www.ontario.ca/page/2019-novel-coronavirus
- [British Columbia testing data to date] http://www.bccdc.ca/about/news-stories/stories/2020/information-on-novel-coronavirus
- [Alberta testing data to date] https://www.alberta.ca/covid-19-alberta-data.aspx
- [Saskatchewan testing data to date] https://www.saskatchewan.ca/government/health-care-administration-and-provider-resources/treatment-procedures-and-guidelines/emerging-public-health-issues/2019-novel-coronavirus/cases-and-risk-of-covid-19-in-saskatchewan
- [Manitoba testing data to date] https://www.gov.mb.ca/covid19/
- [Quebec testing data to date] https://www.quebec.ca/en/health/health-issues/a-z/2019-coronavirus/situation-coronavirus-in-quebec/
- [Newfoundland and Labrador testing data to date] https://www.gov.nl.ca/covid-19/
- [New Brunswick testing data to date] https://www2.gnb.ca/content/gnb/en/departments/ocmoh/cdc/content/respiratory_diseases/coronavirus.html
- [Nova Scotia testing data to date] https://novascotia.ca/coronavirus/#cases
- [Prince Edward Island testing data to date] https://www.princeedwardisland.ca/en/topic/covid-19
- [Yukon testing data to date] https://yukon.ca/en/health-and-wellness/health-concerns-diseases-and-conditions/covid-19-information
- [Northwest Territories testing data to date] https://www.hss.gov.nt.ca/en/services/coronavirus-disease-covid-19
- [Nunavut testing data to date] https://www.gov.nu.ca/health/information/covid-19-novel-coronavirus
