## HAPPY ALMANA - Presentation with Speaker Notes

![](/Slides/Happy_Almana_Capstone_Presentation_Slide_01.png)


***SLIDE 1 — TITLE PAGE***

* Thank you for coming today. 
* We appreciate your joining us to watch our presentations.
* Today my fellow colleagues and I would like to present our Capstone Project.  
* We’re going to share our findings about Happiness across the World…

---
![](/Slides/Happy_Almana_Capstone_Presentation_Slide_02.png)

***SLIDE 2 — CONTENTS***

* Here are the sections of our presentation. proceeds as follows:  
    + We’ll start off with an Introduction 
    + Then move on to Exploratory Data Analysis or EDA
    + Then we look into our Models
    + Next we have a  little Bonus for you 
    + Finally we end with the Outlook for further research and on future developments 

---  

![](/Slides/Happy_Almana_Capstone_Presentation_Slide_03.png)

***SLIDE 3 — INTRO: WORLD HAPPINESS REPORT***

* I’m going to give you a general overview of the data, of what we’re going to be exploring today
* We took the data used for the World Happiness Report  
Which comes out once a year   
* The time period of data is 18 YEARS, 2005 to 2022
* Overall, 165 countries have participated but not every year, from 195 recognized countries worldwide, roughly 84% of take part

---  

![](/Slides/Happy_Almana_Capstone_Presentation_Slide_04.png)

***SLIDE 4 - Aiming & Framing the World Happiness***

* Happiness matters to everyone:
    + On the individual level, we all seek to find happiness.
    + On a national level, happiness is also of interest. 
    + Policy makers of the differing governments want happy productive citizens.  
    * It ensures the well-being of the nation
* Naturally questions arose about happiness
    * Where are folks the happiest, in which countries?
    * Then further: what factors have an influence on happiness levels?
* Hence we aimed to set out to Create a Predictive Model for the Happiness Index

---

![](/Slides/Happy_Almana_Capstone_Presentation_Slide_05.png)

***SLIDE 5 – FEATURES***

* Let’s get to know the features of the dataset:
* The World Health Report is based on surveys from the Gallup World Poll and data from the Worldbank Databank.
* The questions asked the respondents to rank or give a yes/no answer
* The average of their answers were then tallied up for each country
    * First off, we have the *Life Ladder* or *Happiness Index* which is our target or what we want to predict
    * *Social Support* refers to whether or not you have got someone to count on in times of trouble.
    * *Freedom to Make Life Choices* is the response to the question: “Are you satisfied or dissatisfied with your freedom to choose what you do with your life?”
    * *Perception of Corruption*: “Is corruption widespread throughout the government and businesses or not?” 
    * *positive Attitude*: ”Have you experience  a lot of positive emotions (laughing, enjoyment, learning something interesting) yesterday?”
    * *negative Attitude*: “Have you experienced a lot of negative emotions yesterday (worry, sadness, anger)?”
* Factual data about the countries are based on info from the worldbank: 
    + *Healthy life expectancy at birth*: The Average number of years that a person can expect to live in "full health" 
    + *Gdp per capita*:  shows the health of a country's economy. It is the total value of the goods and services produced in a country during a specific period of time, usually a year.

---


![](/Slides/Happy_Almana_Capstone_Presentation_Slide_06.png)

***SLIDE 6 - LIFE LADDER***
 
* The Happiness Index or the Life Ladder (as I mentioned in the slide before) is the target or what we are aiming to predict
* How is it determined?  The individual is asked the following:
    > “The top of the ladder 10 represents the best possible life for you and </br>the bottom of the ladder 0 represents the worst possible life for you. </br>On which step of the ladder do you stand now in your opinion?”


---


![](/Slides/Happy_Almana_Capstone_Presentation_Slide_07.png)

***SLIDE 7 – Further Features Considered***
 
* We brought in  more  variables, We wanted to improve our model’s performance.
* *Crime Index*: perception of crime
* *Health Care Index* is designed to reflect the quality of a healthcare system  
* *Population Density*: people living per sqkm of country
* *Average years of school* for adult of age 25 years or more (from: Human Development Index)
* *Cost of Living Index* in USD
* The *Gini index* measures Inequality of wealth distribution: A Gini index of 0 represents perfect equality, while an index of 100 implies perfect inequality. 
* *Environmental Pollution Index* from Numbeo

---


![](/Slides/Happy_Almana_Capstone_Presentation_Slide_08.png)

***SLIDE 8 — Transition to the EDA***

* I will now move on to exploratory data analysis (EDA) and show some results from the data

---

![](/Slides/Happy_Almana_Capstone_Presentation_Slide_09.png)

***SLIDE 9 - Happiest Countries (2005-2022)***

* You are probably wondering which countries are the happiest? 
* On this Slide you can see the winners since 2005 to 2022.
* As you can see Finland & Denmark are the top countries in terms of happiness index.
* Finland has won 8 times and Denmark has won 7 times, whereas
* Canada, Norway and Switzerland have won just one time each.

---

![](/Slides/Happy_Almana_Capstone_Presentation_Slide_10.png)

***SLIDE 10 – Average Level of Happiness (2005-2022)***

* Let's look where the happiest countries are.
* Since we didn't have all the data for each country and for every year, here we did an average over the whole time span to get an overview.
* The colour gradient represents the level of the Life Ladder.
* The darker the purple, the happier the country.
* The more yellow the country is, the lower the happiness index.

---


![](/Slides/Happy_Almana_Capstone_Presentation_Slide_11.png)

***SLIDE 11 – Average Level of Happiness (2005-2022)***

* As you can see, the happiest countries are to be found in northern Europe and in the north of America 
* Australia and New Zealand are also among the happiest countries. 
* If you look at the African continent, it is very yellow, which means that there are much less happy countries there. 

---


![](/Slides/Happy_Almana_Capstone_Presentation_Slide_12.png)

***SLIDE 12 - CORRELATION TO LIFE LADDER***

* Why are some countries happier than others?
* Which factors could lead to more happiness?
* On this slide you can see the correlation to Happiness Index (Life Ladder).
* The correlation coefficient is a number between 0 and absolute 1 (a negative value means that the variables are inversely related to each other)
* The coefficient indicates how strong the correlation between characteristics and Life Ladder is. 
* The closer to 1, the stronger the correlation, the closer to 0, the weaker.
* And here you can see that we have strong correlation between life ladder and GDP per capita, social support and Healthy life expectancy at birth. 
* But we also have negative correlation between Environment pollution Index and the life ladder. 
* We suspect the reason of the low correlations to the life ladder could be that we didn't have enough Data.
* Which features did we use to predict the target, which model did we use and how it performed, you will see on the upcoming Slides


---

![](/Slides/Happy_Almana_Capstone_Presentation_Slide_13.png)

***SLIDE 13 — Transition to the Modelling Part***

* I will now move on to Modelling Part and show: 
    * which Algorithm we choose 
    * Which variables we selected
    * And how well our model performes

---
![](/Slides/Happy_Almana_Capstone_Presentation_Slide_14.png)

***SLIDE 14 - Baseline Model***

* We ran the base model with the variable with the highest correlation : GDP per Capita.
* We tried several algorithms and chose K-nearest neighbours (KNN). It performed best.
* The idea of the KNN algorithm is that similar things are nearby.
* So, the algorithm searches for a given number of neighbours of a datapoint, Then calculates the average of the neighbours And assigns this target value to the datapoint.
* To evaluate how well our model performed we compared the average error between the predicted life ladder value and actual life ladder value.
* So that would be, namely the *absolute error* and the *percentage error*
* Our Baseline Model has the absolute error of 0.52 and the percentage error of 10,2%
* There is room for improvement..
---
![](/Slides/Happy_Almana_Capstone_Presentation_Slide_15.png)

***SLIDE 15 - Sort Out the Variables …***

* …depending on whether they improve the model or not.
* In the end we identify 7 Variables that made our model better.
* Let’s take a closer look at those variables we decided to keep..


---
![](/Slides/Happy_Almana_Capstone_Presentation_Slide_16.png)

***SLIDE 16 – Best Performance Model***

* We improved the model, that means we minimized the error for the prediction. The selected variables are: 
    * GDP per Capita
    * Social Support
    * Healthy life Expectancy
    * Freedom to make Life Choices
    * Perception of corruption
    * Average Years of School
* Each time we added another variable the error decreased
* We stuck to KNN algorithm. It was superior to the the other algorithms we tried.
* In the Model Performance Table, you can see how we improved the model:
    * The absolute error decreased from 0.52 to 0.29
    * The percentage error decreased from 10.2% to 5.9% 
---
![](/Slides/Happy_Almana_Capstone_Presentation_Slide_17.png)

***SLIDE 17 — Transition to the Bonus Part***

... And now, We have a little bonus…

---
![](/Slides/Happy_Almana_Capstone_Presentation_Slide_18.png)

***SLIDE 18 – Bonus***

* During our project, on World Happiness Day, March 20th 2024, the new the Happiness Report for 2023 was released
* We took this data and looked at it. 
* And we also used it to test our model.

---
![](/Slides/Happy_Almana_Capstone_Presentation_Slide_19.png)

***SLIDE 19 – Happiness Index Europe, 2023***

* The map on the left shows the countries of Europe, coloured according to the level of the Happiness Index. 
* The colour gradient is in the middle of the picture, and you can see, The darker purple the country, the happier it is.
* The chart on the right shows the Happiness Index with bars.

* As we can see, Finland has won again this year with a happiness-index of 7.7.
* In 2nd place is Iceland and in third place is Denmark.
* In the bar plot on the right side we have added our prediction with stars. 
* As you can see, some indices we can predict more accurately, others less so.
* Overall, the average error for our model has not changed, even with the new data. It is still at 5,9%.
* So, our model also works well with new data

---

![](/Slides/Happy_Almana_Capstone_Presentation_Slide_20.png)

***SLIDE 20 — Transition to the last Part***

And now, the last part contains a short summary and our outlook

---
![](/Slides/Happy_Almana_Capstone_Presentation_Slide_21.png)

***SLIDE 21 – SUMMARY***

* The results of our analyses show the following: 
* The happiest European countries are Denmark and Finland
* In the rest of the world the happiest countries are Canada, Israel and New Zealand
* 7 Variable Enhance the Performance of our Predictive Model

---

![](/Slides/Happy_Almana_Capstone_Presentation_Slide_22.png)

***SLIDE 22 – OUTLOOK***

* Expand current research:
* Denmark, Finland,  western countries according to our findings here have gotten it right, so to speak.  
* Let’s dig further into indices and uncover additional factors that can predict and make a better model. 
* A blueprint or template can be made for other countries to follow.  
* What we’ve examined has only scratched the surface
* Our Findings warrant also further understand about the nature and design 
* Inherent flaws due to bias do our western ideals of ranking translate into every culture, 
* Perhaps happiness is not the end all be all? Or the correct metric? 
Is happiness too fleeting momentary and hedonistic?
* Perhaps a clearer more precise definition of happiness is in order:  A differentiation between a life filled with fleeting momentary hedonistic pleasures and one marked by an abiding purpose and deep sense of fulfillment.
* So those a few things we can ponder

---

![](/Slides/Happy_Almana_Capstone_Presentation_Slide_23.png)

Thanks for your Attention!