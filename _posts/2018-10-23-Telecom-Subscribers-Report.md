---
layout: post
title: "Telecom Subscribers Report"
description: "Telecom Subscriber Report"
category: articles
tags: [power, BI, telecom, Subscriber, churn, customer, revenue, rankx]
comments: false
---
 Understanding Subscribers distribution is one of the important aspects of service management. It can be helpful in driving business management and network management strategies. Here I have tried visualizing telecom subscriber report using Microsoft Power BI. It shows how diverse customer profiles are, according to their age, gender, dependencies & the services being consumed also in turn how it contributes to Total Revenue. The clear view of Churn Status (customer stopping/opting out the services) and in depth knowledge of services consumed and revenue impacted/generated by Churned customer can be useful to define new retention plans. This report also gives functionality to view complete data of individual subscribers as well. This dataset is taken from Kaggle (Link mentioned in report)


The first row of visualizations on first page of report is all about the customer profile. Doughnut Chart depicts distribution as per Gender, Dependent, Partner & Senior Citizen account. Chart has labels of Number of customers and gives percentage details when mouse is hovered over it. Like any other PowerBI report this also is interactive report, so clicking on this charts all other charts, tables shows corresponding values. Paperless Billing chart is also included in this row as this is vital in industry to cut down expenditure on this particular category. Though there is no expenditure details present about it in this dataset, I have kept it there.


Second row is simple Column Chart showing which services are being used by how many customers such as Streaming Movies & TV, Internet services, Multiple Lines and Payment Method. Colours if Column chart can be customized that’s is why I have chosen Grey to showcase count of customer having No Internet Service.


Keeping Churn Rate in point of View, third row of visualizations are clustered column charts. Charts consist of Churn Status – Yes and No on X axis and on Y axis is count of customers. Legends are Contract, Device protection, Tech support and lastly distribution as Monthly charges.


Second Page of this report is about the Revenue. Single Row cards and Multi-row cards shows percent breakup of total revenue generated. One Matrix table gives bifurcation of number of customers with Monthly charges and Tenure in Years further divided into Churn Status in column. Another Matrix table is interesting. Considering total charges paid, matrix shows top 5 customer in each Monthly Charges segment. RANKX DAX function and TopN option are used to implement this matrix. Thanks to PowerBI community for helping in writing DAX function. A Table is used to display all customer details. Conditional formatting is used for four important columns like Monthly Charges, Total Charges (Data bar formatting) and Tenure, Churn status (Cell Colour formatting).


A slicer is used here called Churn Status is in sync on both pages. Slicer enables to showcase more focused visualization on entire canvas. All visualizations values are changed as per slicer is selected. Please view report in Fullscreen mode.


<iframe width="800" height="600" src="https://app.powerbi.com/view?r=eyJrIjoiNzQyYTQ5MmMtNmQxMC00YTI0LWJkNmQtNGI2ZmM5OTNmYmM0IiwidCI6IjliOTFmNGY2LWVmM2EtNDFkZS1hNWE4LTJkYTZkYjg2MDkxYSJ9" frameborder="0" allowFullScreen="true"></iframe>