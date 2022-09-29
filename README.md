# **An Analysis of Kickstarter Campaigns**

## *Overview of Project*
This project was launched at the request of **Louise**, a playright who wants to start a crowdfunding campaign for "Fever", her new play. As her proposed budget is somewhat elevated (over $10,000 USD), Louise wanted to make sure that she was setting up a Kickstarter campaign that would be successful. Therefore, we analyzed a dataset that gave us relevant information about the types of crowdfunding campaigns that reach their initial goals. 

### Purpose
The purpose of this project was to analyze a series of crowdfunding campaigns, in order to determine the most succesful strategies for launching them. Specifically, the goal was to find relevant data to help us identify the **key characteristics** of successful theater Kickstarter campaigns.

## *Analysis and Challenges*
The analysis of this project was completed through the use of **Excel**. As stated before, we utilized a dataset that contains information on crowdfunding campaigns from all over the world. As such, the dataset not only holds data on successful campaigns, but also on canceled, failed and ongoing campaigns. 

**One of the first steps** in our analysis was to establish visual tools that would help us to quickly identify campaigns based on their outcome. Therefore, we used conditional formatting to color-code the outcomes in the following manner:
* Successful campaigns: green
* Canceled campaigns: yellow
* Failed campaigns: red
* Live campaigns: blue

After this, we worked on determining **two other factors**: the percentage of funding (according to the initial goal vs. the outcome of each campaign), and the average donation made for each project. The percentage of funding was calculated using a simple rule of three and the **ROUNDUP** formula on Excel, while the average donation was calculated with a division and the **ROUNDUP** and **IF.ERROR** formulas. 

Next, we divided the **Parent Category** and **Subcategory** from the dataset in order to have a more precise analysis on theather campaigns that allowed us to establish a specific filter for "plays". And, lastly, we created three final columns on the dataset that would give us information on **three categories**: the date a campaign was launched, the date it ended and the specific launch year. 

With all of the previous and new information on the dataset, we performed an analysis using **pivot tables**. Some of the information we got was, for example, the amount of successful theater campaigns in the United States (525, as it turns out), or the average number of backers of failed theater campaigns in that same country (and they happen to be only eight). 

However, the information we were most interested in was related to **two specific points**: the outcomes of crowdfunding campaigns based on their launch date, and the outcomes based on their crowdfunding goals. Thus, we will review this information in the next section. 

### Analysis of Outcomes Based on Launch Date
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/113153777/193157497-057b9536-e585-4090-b3d8-49ec4592d9e2.png)

As stated above, we used the information in our dataset to create a pivot table that would allow us to analyze the outcomes of theater campaigns according to their launch month. For this, we established the following:
* The rows would be each month of the year
* For the columns, we would get the "successful", "failed" and "canceled" campaigns. 
* The values would be those of the three categories above. 
* We would filter the information by Parent Category (specifically, theater) and by year. 

### Analysis of Outcomes Based on Goals
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/113153777/193157383-8b794e89-a11c-4c97-a3e2-0e53a80496bb.png)

Another key aspect of our analysis was the outcome of each campaign based on their initial crowdfunding goal. Since Louise's goal was above $10,000 USD, we needed to determine if her objectives were realistic or not. However, instead of using a pivot table for this portion of the analysis, we determined 12 diferent amount ranges (from less than $1000 USD to $50,000 USD or more) and calculated the following aspects through simple divisions and the **COUNTIFS** formula:
* The number of successful campaigns in each range
* The number of failed campaigns
* The number of canceled campaigns
* The percentage of campaigns in each category

### Challenges and Difficulties Encountered
Even though this analysis was not very difficult to perform, there were still a few important challenges. First of all, the amount of data in the set (over 4000 entries) meant that we had to make sure that we covered all the information each time we worked with it. Secondly, as some of the formulas and tools weren´t previously known by the team, the analysis was perfomed on a slower pace to ensure that every key activity was covered. And, finally, there were some setbacks related to Excel formulas that weren´t perfomed correctly initially, which also slowed down the work rhythm as the team determined the correct use of them. The most difficult formula to use was, specifically, **COUNTIFS**.  

## *Results*

- What are two conclusions you can draw about the Outcomes based on Launch Date?

Firstly, we can conclude that the most successful theater campaigns are launched during the summer months. The most successful month seems to be may, followed by june and july. A possible explanation for this could be that, during the summer, people tend to be on a better mood because of the warmer weather. This could, in turn, make them feel more generous towards artistic campaigns. 

The second conclusion we can draw about the Outcomes based on Launch Date is that the most difficult months for campaigns are december and january. Again, a possible explanation for this could be that a cold weather doesn´t lead to a happy, generous mood. However, a much stronger theory could be that, since these are the months surrounding Christmas, people don´t have a lot of money to spare for campaigns. 

- What can you conclude about the Outcomes based on Goals?

The Outcomes based on Goals analysis gives us relevant insight on the types of objectives that are realistic for crowdfunding campaigns. First of all, it seems that the most successful campaigns are those that ask for less than $1000 USD. Another very successful portion of campaign asks for between $1000 and $4999 USD. Louise´s objective is over $10,000 USD, which means that she will have to evaluate if this is a sound objective to have, as those campaigns are usually 54% successful. On the other hand, it also seems that the least successful campaigns are those that ask for between $45000 and $49999 USD, followed by those that ask for $50000 USD or more. 

- What are some limitations of this dataset?

Although this dataset helps us get a general idea of the key characteristics of successful crowdfunding campaigns, there are other elements that could determine a campaign's success that can't be determined through the available information. Other important aspects to take into account could be, for example, the marketing strategy surrounding the campaign, or the types of backers each campaign has (is it people who have higher income, or is it people who have an average salary?). Having information like this could really help Louise develop a much more precise strategy for her crowdfunding campaign. 

- What are some other possible tables and/or graphs that we could create?

Other tables and/or graphs we could create for this analysis could be:
* The average donation vs. the outcomes (this could help us determine, indirectly, the average income for backers). 
* The outcomes based on goals, but only for theater campaigns in the US. 
* A boxplot containing the mean, median, standard deviation and quartiles. 
* The average amount of time between the launch and the closing of successful campaigns (we could use a line graph for this). 


