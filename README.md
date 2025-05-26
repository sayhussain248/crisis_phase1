*Humanitarian Needs and Funding from 2010 to 2024* 

This project is an Exploratory Data Analysis on a dataset derived from United Nations Office for the Coordination of Humanitarian Affairs. This dataset tracks humanitarian aid in USD as well as the amount of people in need of aid across major crisis countries. 
There is a total of 66 major crisis countries: 

 AFG - Afghanistan

BGD - Bangladesh

BFA - Burkina Faso

BDI - Burundi

BEN - Benin

CMR - Cameroon

CAF - Central African Republic

TCD - Chad

CIV - Côte d'Ivoire (Ivory Coast)

CUB - Cuba

PRK - North Korea (Democratic People's Republic of Korea)

COD - Democratic Republic of the Congo

DMA - Dominica

GMB - Gambia

GTM - Guatemala

HND - Honduras

DJI - Djibouti

ETH - Ethiopia

COL - Colombia

HTI - Haiti

KGZ - Kyrgyzstan

LBR - Liberia

IDN - Indonesia

IRN - Iran

IRQ - Iraq

LKA - Sri Lanka

LSO - Lesotho

MDG - Madagascar

KEN - Kenya

LBY - Libya

MNG - Mongolia

MOZ - Mozambique

MRT - Mauritania

MLI - Mali

ECU - Ecuador

MMR - Myanmar (Burma)

NAM - Namibia

NER - Niger

NPL - Nepal

PER - Peru

SLW - Eswatini (formerly Swaziland)

NGA - Nigeria

PSE - Palestine

NIC - Nicaragua

PAK - Pakistan

PHL - Philippines

COG - Republic of the Congo

SEN - Senegal

SOM - Somalia

SSD - South Sudan

JOR - Jordan

LBN - Lebanon

SDN - Sudan

SYR - Syria

UGA - Uganda

UKR - Ukraine

VUT - Vanuatu

VEN - Venezuela

YEM - Yemen

ZWE - Zimbabwe

TZA - Tanzania

TGO - Togo

ZMB - Zambia

SLV - El Salvador

MWI - Malawi

TUR - Turkey

**Metrics Measured**


For these countries, 4 metrics were measured: 
* People in Need (PIN)
 * People Targeted
* Funding Requirements
* Funding Recieved 
 
 Some of these countries did not have data from 2010 all the way to 2024. Others had data that was sparse. 
 The purpose of this project was to explore how humanitarian aid needs and funding has changed over time and for select countries. 

<hr>

### vanessa_eda.ipnyb

This notebook focuses on two questions: one univariate and one bivaraite. 

#### The univariate question is "Which countries consistently had the highest People in Need (PiN) between 2010 and 2024?" 
This notebook aggregated the total amount of people in need for each country and ranked those countries from most amount of People in Need to least amount of People in Need. The top 5 countries was used to create a visualization tracking the change in the amount of People in Need over time. 

#### The bivariate question is "What is the relationship between the amount of people in need and the amount of people targeted for the top 5 countries with the most amount of people per metric?"
This notebook creates a pivot table for the total numbers of people in need and people targeted for every country and turns it into a dataframe. The countries are ranked based on the sum of these two metrics. A graph for the top 5 are for better details. Stacked bar charts were created for both the top 5 and all countries. Both graphs show that the numbers of people targeted are consistently lower than the number for people in need.

<hr>

### tinu_eda.ipnyb

#### The Univariate Analysis: Which year had the most amount of people in need from 2010 to 2024?
This analysis examines a dataset containing the number of people in need from 2010 to 2024 to determine which year had the highest recorded need. 
The goal is to perform a univariate analysis (single-variable analysis) on the yearly data to identify trends and the peak year.

Key Questions:
1. Which year between 2010 and 2024 had the highest number of people in need?

2. How has the trend changed over the years?

#### The Univariate Analysis:How have global humanitarian needs (People Targeted, People in Need) evolved from 2010 to 2024? 
This analysis explores how global humanitarian needs have changed between 2010 and 2024, focusing on two key metrics:

People in need: Total population requiring humanitarian assistance.

People targeted: Those actually receiving aid due to funding.

The goal is to perform a univariate analysis (examining each variable separately) to identify trends, peak years, and changes over time.

Key Questions:
1. How have People in need and People targeted evolved over 2010-2024?

2. Which years had the highest recorded humanitarian needs?

3. Is there a widening gap between PiN and People targeted (unmet needs)?

<hr>

### sayeda_eda.ipnyb*

 This notebook focused specifically on tracking how Funding Requirements changed in relation to People in Need for Afghanistan and Syria. Afghanistan was chosen because it had the most amount of data for throughout the years ranging from 2010 to 2024, with the exception of 2016 for Funding Requirements. Syria was also chosen because it ranked the highest on the most people in need, despite their data points ranging more from 2018-2024.

<hr>

### yuzhuang_eda.ipnyb

This notebook focuses on 1 question for each univariate and bivaraite.
* univariate:
  * How have global humanitarian needs Funding Requirements and Funding Received evolved from 2010 to 2024?
* bivaraite:
  * What was the relationship between Funding received and Funding requirements across by year?
  
Both question for this note book is try the found out if there is a relationship between Funding Requirements and Funding Received. In crises, the efficient and equitable allocation of resources is critical. By examining this relationship, we seek to understand whether funding needs are being met proportionally and to identify patterns of underfunding or oversupply across different appeals or sectors. The findings from this analysis may help inform policymakers and aid organizations in making more data-driven, equitable funding decisions.

<hr> 


## WRITE UP

**Univariate** 

*Which countries consistently had the highest People in Need (PiN) between 2010 and 2024?*


When ranked by the total number of people in need for all years, Syria has the highest number. However, in the graph of the countries ranked top 5 in the number of People in Need, we can see that Afghanistan and Democratic Republic of the Congo have data spanning spanning from early-2010s to 2024 even though they do not have the highest ranks. Therefore, the two countries more consistently had the highest people in need between 2010 and 2024.

*Which year between 2010 and 2024 had the highest number of people in need?*


The year with the highest number of people in need between 2010-2024 was 2023, with 975,016 individuals requiring assistance.

*How has the trend changed over the years?*


The overall trend shows: Consistent increase in humanitarian needs over the year. The number of people in need grew by approximately 475,016 individuals (95% increase) from 2010 to 2023.

2020-2023 saw particularly sharp increases, possibly due to: COVID-19 pandemic impacts, Escalating global conflicts and Climate-related disasters.

*How have People in need and People targeted evolved over 2010-2024?*
From 2010-2024, People in Need (PiN) grew dramatically (peaking at 40.1M) while People Targeted reached only 14.7M at best, covering just 7.5% of needs on average. 

*Which years had the highest recorded humanitarian needs?*
The highest needs occurred in 2023 (40.1M), followed by 2022 (~38M) and 2021 (~35M).

*Is there a widening gap between PiN and People targeted (unmet needs)?*
The gap between needs and responses widened severely, with unmet needs growing 50-fold from 2010 (500K) to 2023 (25.4M), as targeting consistently failed to keep pace with escalating crises.

*How have global humanitarian needs Funding Requirements and Funding Received evolved from 2010 to 2024?*

Based on the histogram, we can see that global humanitarian funding requirements have been increasing over the years, especially from 2021 to 2024. The upward trend was most notable between 2017 and 2019, reaching the maximum value during this period. This may reflect the growing severity of global humanitarian crises.

Global humanitarian funding received has also been increasing, reaching the maximum value in 2019. However, the gap between requirements and received funding has been steadily widening. For example, in 2018, the gap was around 50%, whereas by 2019, it had exceeded 50%.



**Bivariate**

 *What is the relationship between the amount of people in need and the funding requirements for Afghanistan from 2010 to 2024?*

 
 The bivariate analysis shows a *strong, positive* correlation between the amount of people in need and funding requirements for Afghanistan from 2010 to 2024. That is, as the amount of people in need increased over the years, so did the amount of funding requirements to support them. This is a very strong correlation, given that the pearson's correlation coefficient is 0.852583. 
 
 *What is the relationship between the amount of people in need and the funding requirements for Syria from 2018 to 2024?*

 
 The bivariate analysis shows a *strong, positive* correlation between the amount of people in need and funding requirements for Afghanistan from 2018 to 2024. That is, as the amount of people in need increased over the years, so did the amount of funding requirements to support them. This is a very strong correlation, given that the pearson's correlation coefficient is  0.748505.  

*What was the relationship between Funding received and Funding requirements across by year?*
 
 
 The scatter plot reveals a strong linear relationship between funding requirements and funding received across years. As funding needs increase, the received funding tends to rise proportionally. This is supported by a Pearson correlation coefficient of approximately 0.911078, indicating a very strong positive correlation. Therefore, we can conclude that there is a consistently strong relationship between the level of funding requirements and the funding provided over time. 
 However, this relationship analysis is biased because of the lack of received funding data from 2022 to 2024, which causes data anomalies and thus results in biased outcomes.
 
 
*What is the relationship between the amount of people in need and the amount of people targeted for the top 5 countries with the most amount of people per metric?*


In both the stacked bar graphs for the top 5 countries and all the countries in the dataset, we see that the numbers for People targeted are consistently lower than People in need.


