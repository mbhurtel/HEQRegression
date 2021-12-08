# Project Title: Home equity value empowered housing marketplace

In this document, we present all the activities we carried out while developing a project “Home equity coin empowered housing marketplace”. We mainly worked to develop linear regression model to predict housing price which is then used to calculate home equity value.

### Project Description:
The current housing marketplace policy and practice has brought considerable insecurities to most house owners particularly those with no money at hand. The price of houses is governed by several factors. Sometimes, the property tax rises so sharply that it becomes extremely hard for the house owners to pay the yearly tax. In such a situation, owners will have the option either to sell the property and leave the place and neighbourhood or apply for a home equity line of credit (HELOC) to pay the tax. The first option is not as easy as it sounds. The owner may not only need to leave a good neighbourhood, a good school for the children but also may leave the current job. However, for the low-income owners, the second option might not be even an option. For the owners who pay tax using HELOC, if they could not pay the bill for the credit in time, they are likely to be charged with interest, and further, it might impact their credit score too. 
So, the “Home equity coin empowered housing marketplace” project considers all the raised issues and incorporates the digital currency concept (equity coin) to provide a flexible but effective financial option for house owners. House owners can generate digital coins based on the house equity value and use the coins as an equivalent of cash to pay property tax and others. Further, the equity coin will not depend on the credit score and neighbourhood. The proposed project has the potential to transform the existing housing marketplace not only by benefitting the house owners but also benefitting other stakeholders including the community as well. 

### Project Goals:
The tentative goals of the intended project are as follows:

1. To identify the major issues with the current housing marketplace.

2. To assess the potential of incorporating the equity coin concept.

3. To apply the equity coin on top of the housing marketplace.

## User Audience Analysis and User Personas
#### User Group List:
Incorporating the equity coin is likely to add a few user groups to the existing housing marketplace. The potential user groups for the project are: 

* House Owners - Existing house owner who can sell a house
* Buyers - Potential owner 
* System Administrator - Person who maintains the house marketplace system and audits the behaviour of all users
* Community Representative - A person who manages donations received from the proposed system

#### User Matrix for Home equity coin empowered housing marketplace
The following table shows probable user groups for the proposed system and their knowledge, experience, skills, software experience, and frequency of use.

![](assets/images/user_matrix.png)

<b>Table: User Matrix</b>

### User Personas
Here are user personas for different group of users presented above. The firsts user persona is created by grouping two categories of users which are real **state provider (seller/owner) and consumer (buyer)** into one as the same buyer will be turned into sellers while selling the house. Rest of the personas belong to **Administrator** and **Community Representative** respectively. 

![](assets/images/user_persona1.png)

<b>Fig: User persona for user group “state provider (seller/owner) and consumer (buyer)”</b>


![](assets/images/user_persona1.png)

<b>Fig: User Persona for “Administrator”</b>


![](assets/images/user_persona1.png)

<b>Fig: User Persona for “Community Representative”</b>


## Use Cases, User Scenarios & Requirements
### INTRODUCTION AND MOTIVATION:
We are in the phase of developing a minimalistic **‘Home Equity (HEQ) Coin’**. The HEQ coin is directly connected to the price of a house in a neighbourhood i.e., if there is increase in the housing price, or the buyers are ready to invest more in the house, then **tentatively, the price of HEQ coin may rise**. Similarly, if the house seller is in immediate need of money, and sells the house in price lower than the current price, then **the value of the house will decrease, and correspondingly the value of HEQ coin will decrease**. Therefore, there is a significant need to predict the housing price, as per the past data, which will help the house seller/buyer to sell/buy the house in **right time, and in right price**. In this context, the **use of regression models** will be the best fit in our scenario.
In short, we train our regression model on the historical data of houses, and use the model to predict the housing price using the new data entered by user. And if the error in prediction is more than the acceptable range, then we will update the model to incorporate the error. This is similar to the working of **Zestimate** in Zillow. In our case, the dataset is **provided by Zillow** which provides plenty of historical information about the housing prices and their features. The data can be categorized as “Interior Housing Data” and “Exterior Housing Data” as follows:

<img align="right"  src="assets/images/interior_data.png">
#### Interior Housing Data:
* Total Rooms
* Total Bedrooms
* Total Bathroom
* Heating
* Air-Conditioning (AC) 
* Fireplace
* Water
* Sewer

<!--![](assets/images/interior_data.png)-->


#### Exterior Housing Data:
<img align="right"  src="assets/images/exterior_data.png">
* Condition
* Architectural Style
* Total Stories
* Zoning Descriptions
* Size (acre)
* Size (sq. ft.)
* Topography
* Year Built
* Market Land Value [A]
* Market Improvement Value [B] 
* Market Total Value ([C] = [A] + [B])

Furthermore, the price of the house can be predicted using other features like tax records, built year, nearby by schools and universities, nearby markets, granite countertops in kitchen, windows placement, spacious patio, etc.

### USE CASE DIAGRAM
Our system can be broadly divided into two parts i.e., Model Training Phase and Model Inferencing Phase. The use cases in our system are as follows:

![](assets/images/use_case_diagram.png)

