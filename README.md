<a name="readme-top"></a>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#project-overview">Project Overview</a></li>
    <li><a href="#project-flowchart">Project Flowchart</a></li>
    <li><a href="#project-organization">Project Organization</a></li>
    <li><a href="#dataset">Dataset</a></li>
    <li><a href="#credits-and-references">Credits And References</a></li>

  </ol>
</details>

<!-- Project Overview -->
## Project Overview

Student Retention Model
=========================

**Predicting student if they are at-risk of dropping out of college**

What if we can recognize clues and patterns that precede college student dropouts using data science and machine learning?
Given the right set of data of a student population consisting of both college drop outs and graduates, can we leverage predictive analytics to forecast student withdrawal actions?
When we study historical data of both kinds of student populations: - those that have discontinued their post-secondary education; - and also, those that have graduated and completed a degree; we hope to identify related factors and challenges for at-risk students.   

Addressing proactively the challenges faced by these students is the key!
Having early identification allows for a timely intervention and implement support strategies so students can overcome academic challenges and succeed in their education journey.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ### Walkthrough Demo -->

### Project Flowchart
<br />
<div align="center">
  <a>
    <img src="images/CapstoneSprint1_ Project Work Flow.jpg" width="300" height="500">
    </a>
</div>

<p align="right">(<a href="#readme-top">back to top</a>)</p>


### Project Organization
<a name="data"></a>
* `data` 
    - [Data.csv](https://drive.google.com/file/d/1g-bVWHObcPFhSpUs4lNxAriqcH9iOHoS/view?usp=drive_link)
    - [Data Dictionary](data/Data_Dictionary.xlsx)
<!-- 
* `model`
    - joblib dump of final model / model object -->

* `notebooks`
    - [Sprint 1 Preliminary EDA](notebooks/Sprint1PreliminaryEDA.ipynb)
    - [Sprint 2](notebooks/CapstoneSprint2.ipynb)
<!-- 
* `reports`
    - contains final report which summarises the project -->

* `references`
    - [Sprint 1 Presentation Slides](slides/CapstoneSprint1StudentRetentionModel.pptx)
    - [Sprint 2 Presentation Slides](slides/CapstoneSprint2StudentRetentionModel.pptx)
<!-- 
* `src`
    - Contains the project source code (refactored from the notebooks)

* `.gitignore`
    - Part of Git, includes files and folders to be ignored by Git version control

* `capstine_env.yml`
    - Conda environment specification

* `Makefile`
    - Automation script for the project
-->
* `README.md`
    - [ReadMe](README.md)
<!-- 
* `LICENSE`
    - Project license -->

### Dataset

Historical anonymized data of enrolled students spanning 10 years containing some features about the student that will hopefully support insights on the predictability of academic withdrawal.

| Variable Name                                  | Type          | Description                                                            |
|------------------------------------------------|---------------|------------------------------------------------------------------------|
| Admission grade                                | Continuous    | Admission grade (between 0 and 200)                                    |
| Age at enrollment                              | Integer       | Age of student at enrollment                                           |
| Application mode                               | Integer       | Nominal Category Range: 1 - 1st phase - general contingent to 57 - Change of institution/course (International) |
| Application order                              | Integer       | Application order (between 0 - first choice; and 9 last choice)        |
| Course                                         | Integer       | Nominal Category Range: 33 - Biofuel Production Technologies to 9991 - Management (evening attendance) |
| Curricular units 1st sem (approved)            | Integer       | Number of curricular units approved in the 1st semester                |
| Curricular units 1st sem (credited)            | Integer       | Number of curricular units credited in the 1st semester                |
| Curricular units 1st sem (enrolled)            | Integer       | Number of curricular units enrolled in the 1st semester                |
| Curricular units 1st sem (evaluations)         | Integer       | Number of evaluations to curricular units in the 1st semester          |
| Curricular units 1st sem (grade)               | Integer       | Grade average in the 1st semester (between 0 and 20)                   |
| Curricular units 1st sem (without evaluations) | Integer       | Number of curricular units without evaluations in the 1st semester     |
| Curricular units 2nd sem (approved)            | Integer       | Number of curricular units approved in the 2nd semester                |
| Curricular units 2nd sem (credited)            | Integer       | Number of curricular units credited in the 2nd semester                |
| Curricular units 2nd sem (enrolled)            | Integer       | Number of curricular units enrolled in the 2nd semester                |
| Curricular units 2nd sem (evaluations)         | Integer       | Number of evaluations to curricular units in the 2nd semester          |
| Curricular units 2nd sem (grade)               | Integer       | Grade average in the 2nd semester (between 0 and 20)                   |
| Curricular units 2nd sem (without evaluations) | Integer       | Number of curricular units without evaluations in the 2nd semester     |
| Daytime/evening attendance                     | Integer       | 1 – daytime; 0 - evening                                               |
| Debtor                                         | Integer       | 1 – yes; 0 – no                                                         |
| Displaced                                      | Integer       | 1 – yes; 0 – no                                                         |
| Educational special needs                      | Integer       | 1 – yes; 0 – no                                                         |
| Father's occupation                            | Integer       | Occupation.  Nominal Category Range: 0 - Student to 195 - Street vendors (except food) and street service providers |
| Father's qualification                         | Integer       | Education Level.  Nominal Category Range: 1 - Secondary Education - 12th Year of Schooling or Equivalent to 44 - Higher Education - Doctorate (3rd cycle) |
| GDP                                            | Continuous    | GDP                                                                    |
| Gender                                         | Integer       | 1 – male; 0 – female                                                    |
| Inflation rate                                 | Continuous    | Inflation rate (%)                                                     |
| International                                  | Integer       | 1 – yes; 0 – no                                                         |
| Marital Status                                 | Integer       | Marital Status. Nominal Category Range: 1- single to 6 - legally separated |
| Mother's occupation                            | Integer       | Occupation.  Nominal Category Range: 0 - Student to 195 - Street vendors (except food) and street service providers |
| Mother's qualification                         | Integer       | Education Level.  Nominal Category Range: 1 - Secondary Education - 12th Year of Schooling or Equivalent to 44 - Higher Education - Doctorate (3rd cycle) |
| Nationality                                    | Integer       | Nationality. Nominal Category Range: 1 - Portuguese to 109 - Colombian |
| Previous qualification                         | Integer       | Education Level.  Nominal Category Range: 1 - Secondary Education - 12th Year of Schooling or Equivalent to 44 - Higher Education - Doctorate (3rd cycle) |
| Previous qualification (grade)                 | Continuous    | Grade of previous qualification (between 0 and 200)                     |
| Scholarship holder                             | Integer       | 1 – yes; 0 – no                                                         |
| Target                                         | Categorical   | Target: formulated as a three category classification task (dropout, enrolled|
| Tuition fees up to date|	Integer|	1 – yes 0 – no	|
|Unemployment rate|	Continuous|	Unemployment rate (%)|



### Credits And References

* [Learnopoly College Dropout Rate Statistics](https://learnopoly.com/college-dropout-rate/)
* [Educationdata.org College Dropout Rates](https://educationdata.org/college-dropout-rates)
* [Data Source: Predict Students Dropout and Academic Success](https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

