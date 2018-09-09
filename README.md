## Analyze A/B Test Results


[![](https://img.shields.io/badge/linkedin-@Shilin_Li-orange.svg?colorA=abcdef&logo=data:image/jpeg;base64,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)](https://www.linkedin.com/in/shilin-li-40474777/)
[![](https://img.shields.io/badge/Udacity-@Shilin_Li-yellow.svg?colorA=abcdef&logo=data:image/png;base64,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)](https://printer.udacity.com/v2/certificate/DR4VPD7H/download)


### Introduction


A/B tests are very commonly performed by data analysts and data scientists. For this project, the goal is to understand the results of an A/B test run by an e-commerce website. 



![alt text](https://github.com/Shilin0806/Analyze_A-B_Test_Results/blob/master/A_B_test.jpg)

Image is adapted from a copyright-free website: https://www.pexels.com/royalty-free-images/.


The company has developed a new web page in order to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product. Current work is to help the company understand if they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.


| Table of Contents |
| :--- |
| <a href='#Prerequisites'> Prerequisites </a> 🔍📜 | 
| <a href='#Design'> Design </a>  📐 |
| <a href='#Conclusions'> Conclusions </a>  📌 |
| <a href='#License'> License </a> 🔖 |


<a id='Prerequisites'></a>

### Prerequisites


![](https://img.shields.io/badge/platform-ios-green.svg?colorA=abcdef)


- Python 3.6.3
- Jupyter Notebook
- Anaconda-Navigator


<a id='Design'></a>

### Design


![](https://img.shields.io/badge/language-Python-orange.svg)


**_Step One_** - Compare


Through mathematics calculation to find out the conversion rates difference between new and old pages.


**_Step Two_** - A/B test


Further examine with an A/B test to see if the results match arithmetic analyze.


**_Step Three_** - Analyze


Investigate the impact of countries on P-value and hypothesis.


<a id='Conclusions'></a>

### Conclusions


- Through comparison, there is a decreasing of conversion rates in new pages versus old ones. A/B test confirmed  new page's poorer performance, thus we don't have enough evidence to reject the null hypothesis, suggesting new pages has no advantages over old ones on conversion rates.
- We had also noticed that country did have some bearing on conversion rate, but not high enough to be  statistically significant.
- In sum, I would suggest the e-commerce company at least not to consider the current new page, but trying to figure out the reason of its poor performance in order to launch another feasible page.


<a id='License'></a>

## License 


[![MIT Licence](https://badges.frapsoft.com/os/mit/mit.svg?v=103)](https://github.com/Shilin0806/Analyze_A-B_Test_Results/blob/master/LICENSE)


