<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/harmeetgill/capstone_project">
    <img src="https://camo.githubusercontent.com/7818eb78e231aedb0e98e27cf1335f1c3093a4c5a5aa7264c355e6b66f255888/687474703a2f2f696d6775722e636f6d2f315a63527972632e706e67" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Prediction of salaries based on features of the job</h3>

  <p align="center">The aim of this project was to determine the most important industry factors in predicting salary amounts.
    <br />
    <a href="https://github.com/harmeetgill/capstone_project"><strong>Explore the docs »</strong></a>
    <br />
    <br />
  </p>
</p>


<!-- ABOUT THE PROJECT -->
## About The Project

### Data collection
Job listings across 15 cities in England were scraped from a job employment website. Terms such as ‘Data Scientist, Data Analyst, Machine Learning’ were used to scrape the site. Features such as company, salary, job title, location and job description were targeted.

### EDA and cleaning
Salary amounts were isolated and standardised to annual salaries. For those salaries which advertised as a range, a mean was taken. The salaries were then split based on the median salary amount; salaries above median were classed as 'high' and those below were classed as 'low' posing a binary classification problem. Salary distribution analysis reveals the median salary to be £28,000 with annual salaries advertised the most, followed by hourly rates and then daily.

### Modelling and key findings
Models used for this project include logistic regression, KNN and random forest. <br>

Models were run with location only or location and job title together. With only location as a feature, CV scores for all three models were similar (0.6), while logistic regression and random forest achieved a test score of 0.64 versus 0.61 for KNN. The F1 scores for the low salary class were higher in all models (0.72-0.73), while high salary class achieved an F1 score bewteen 0.5-0.6 with KNN achieving the higher score. Perhaps unsurprisingly, locations such as London and Cambridge influced salary class the most.

Job title and location features together achieved higher scores: CV scores were between 0.62 and 0.59 with logisitic regression achieving the highest score. Test scores were between 0.62 and 0.66 with again, logistic regression achieving the highest score. Logisitic regression achieved the highest F1 scores (0.86 and 0.83 for low and high salaries, respectively), while random forest achieved scores of 0.78 and 0.56 for low and high salary classes, respectively. The KNN model reported a 100% test accuracy. Key terms of importance which were highlighted were "London", "Cambridge" and "Data Scientist". 

#### Conclusion
The outcomes of these models report known trends when it comes to the job market - cities with a higher cost of living generate higher paying jobs.

#### Limitations and future work
Scraping resulted in a diverse list of locations. Such locations must be consolidated into perhaps counties or assigning each town, region or borough to the nearest city. This could be done by taking lists of all english regions and town, matching to scraped locations and assigning a county or city. A second limitation is the number of jobs scraped, as indicated my KNN's 100% accuracy with only two features taken as input. A third limitation is the number of features isolated from the job description; company name, company rating or sector could also have been included.

#### Project contents:
**Data collection**<br>
[indeed_project_book1.ipynb](https://github.com/harmeetgill/webscraping_project/blob/main/indeed_project_book1.ipynb)<br>

**EDA**<br> 
[indeed_project_book2_new.ipynb](https://github.com/harmeetgill/webscraping_project/blob/main/indeed_project_book2_new.ipynb)<br>

**Modelling**<br> 
[indeed_project_book3_modelling-Copy1.ipynb](https://github.com/harmeetgill/webscraping_project/blob/main/indeed_project_book3_modelling-Copy1.ipynb)<br>

<!-- CONTACT -->
## Contact

LinkedIn: https://linkedin.com/in/harmeetgill28/ 






<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/harmeetgill/repo.svg?style=for-the-badge
[contributors-url]: https://github.com/harmeetgill/repo/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/harmeetgill/repo.svg?style=for-the-badge
[forks-url]: https://github.com/harmeetgill/repo/network/members
[stars-shield]: https://img.shields.io/github/stars/harmeetgill/repo.svg?style=for-the-badge
[stars-url]: https://github.com/harmeetgill/repo/stargazers
[issues-shield]: https://img.shields.io/github/issues/harmeetgill/repo.svg?style=for-the-badge
[issues-url]: https://github.com/harmeetgill/repo/issues
[license-shield]: https://img.shields.io/github/license/harmeetgill/repo.svg?style=for-the-badge
[license-url]: https://github.com/harmeetgill/repo/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/harmeetgill28

