This repo contains a project that predict Customer Lifetime Value of Airline customer by RFM Model to serve the project for my Data Scientist course. In addition, I also write [a blog](https://medium.com/@phanthuy19898/customer-lifetime-value-prediction-c3c983a1a91d) about the process I did and results I got after doing this project.

<b>Project Motivation</b>

Acquisition new customers costs 5 times more than retaining old customers, so marketing measures to retain customers are popular such as campain sending discount vouchers, sending ads, etc. However, the cost of sending mass marketing is very expensive. Instead, we can focus on some potential customers based on indicators such as Lifetime Value. CLV is an importance index in marketing and I am quite interested in it.

<b>Acknowledgements</b>

Dataset used in this project is part of Vietnam Airline Customer transaction dataset which I extract and cannot leak customer's infomation so I only take the card number, the day transaction and the money).

Where I read about the idea of [CLV and RFM](https://www.stacktome.com/blog/diving-deeper-into-customer-segmentation-rfm-and-clv#how-can-rfm-segmentation-increase-customer-value-and-loyalty)

[Buy Til You Die Model](https://towardsdatascience.com/customer-behavior-modeling-buy-til-you-die-models-6f9580e38cf4) - a probabily model can predict CLV, different than other ML model that I know before.


<b>Description</b>

This includes the main file containing the code - Final.ipynb and dataset files.

In which I use supporting libraries such as:

* numpy and pandas - a data processing and calculation library
* seaborn and matplotlib - a library that supports data visualization
* scikit learn - a library that supports machine algorithms learning as well as model evaluation (In this project I use KMeans, XGB and Random Forest algorithms)
* lifetime - library that supports probability Buy Til You Die model

<b>Summary of the results</b>

After clustering, it is possible to segment customers into different clusters to understand which customer clusters need attention.
Regarding CLV, comparing the results shows that the XGB model gives more accurate prediction results. In addition, Vietnam Airlines has tried to apply marketing messages to a group of customers whose CLV is predicted to be over 50.000.000VND instead of sending the whole customer, customer feedback shows that CLV prediction is quite effective.
To improve this prediction, I would also try to subdivide customer groups by characteristics (cohort model) to see if the groups have a common CLV range or have common characteristics to predict CLV.
