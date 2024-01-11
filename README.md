# Marketing-Analysis
Marketing Analysis for CodeX a German beverage company using PowerBI

**Direct Link to the Dashboard** : https://www.novypro.com/project/marketing-analysis-4
## Problem Statement
CodeX is a German beverage company that is aiming to make its mark in the Indian market. A few months ago, they launched their energy drink in 10 cities in India. Their Marketing team is responsible for increasing brand awareness, market share, and product development. They conducted a survey in those 10 cities and received results from 10k respondents.
## Metadata
This file contains all the meta information regarding the columns described in the CSV files. We have provided 3 CSV files:
1. dim_respondents
2. dim_cities
3. fact_survey_responses

-------------------------------------------------------
Column Description for dim_respondents:
-------------------------------------------------------

Respondent_ID: This column represents the unique identifier assigned to each respondent in the survey.

Name: This column represents the name of the respondent who participated in the survey.

Age_Group: This column represents the categorized age group of the respondent. Age groups (15-18, 19-30, 31-45,46-65,65+)

Gender: This column represents the gender of the respondent. (Male, Female, Non-binary)

City_ID: This column represents the ID of the city where the respondent is located.

----------------------------------------------
Column Description for dim_cities:
----------------------------------------------
City_ID: This column represents the ID of the city.

City: This column represents name of the city where the respondent is located. ("Delhi","Mumbai", "Bangalore","Chennai", "Kolkata","Hyderabad", "Ahmedabad","Pune","Jaipur", "Lucknow")

Tier: This column represents the tier category of the city 

--------------------------------------------------------------
Column Description for fact_survey_responses:
--------------------------------------------------------------

Response_ID: This column represents the unique identifier assigned to each response in the survey.

Respondent_ID: This column represents the unique identifier assigned to each respondent who provided the survey response.

Consume_frequency: This column represents the response received for the below question.

	How often do you consume energy drinks?
		Daily
		2-3 times a week
		Once a week
		2-3 times a month
		Rarely

Consume_time: This column represents the response received for the below question.

	When do you typically consume energy drinks?
		Before exercise
		To stay awake during work/study
		For mental alertness
		Throughout the day

Consume_reason: This column represents the response received for the below question.

	What are the main reasons for consuming energy drinks?
		Increased energy and focus
		To combat fatigue
		To boost performance
		To enhance sports performance
		Other


Heard_before: This column represents the response received for the below question.

	Have you heard of our energy drink before today?
		Yes
		No

Brand_perception: This column represents the response received for the below question.

	What do you think of the brand name/logo/design?
		Positive
		Neutral
		Negative

General_perception: This column represents the response received for the below question.

	What is your perception of energy drinks in general?
		Healthy
		Effective
		Dangerous
		Not sure

Tried_before: This column represents the response received for the below question.

	Have you ever tried our energy drink before?
		Yes
		No

Taste_experience: This column represents the response received for the below question.

	If yes, how would you rate the taste, flavor, and overall experience?
		1 (Poor)
		2 (Below average)
		3 (Average)
		4 (Good)
		5 (Excellent)

Reasons_preventing_trying: This column represents the response received for the below question.

	If no, what are the main reasons preventing you from trying it?
		Not available locally
		Not interested in energy drinks
		Unfamiliar with the brand
		Health concerns
		Other

Current_brands: This column represents the response received for the below question.

	Which energy drink brands do you currently consume or prefer?
		CodeX
		Cola-Coka
		Bepsi
		Gangster
		Blue Bull
		Sky 9
		Others

Reasons_for_choosing_brands: This column represents the response received for the below question.

	What are the reasons for choosing those brands over others?
		Brand reputation
		Taste/flavor preference
		Effectiveness
		Availability
		Other

Improvements_desired: This column represents the response received for the below question.

	What improvements would you like to see in energy drinks currently available in the market?
		Reduced sugar content
		More natural ingredients
		Wider range of flavors
		Healthier alternatives
		Other


Ingredients_expected: This column represents the response received for the below question.

	What ingredients do you expect in an energy drink?
		Caffeine 
		Vitamins 
		Sugar
		Guarana

Health_concerns:  This column represents the response received for the below question.
	
	Are you concerned about the health impacts of energy drinks?
		Yes
		No

Interest_in_natural_or_organic:

	Would you be interested in an energy drink with natural or organic ingredients?	
		Yes
		No
		Not Sure


Marketing_channels: This column represents the response received for the below question.

	Which marketing channels or platforms do you often come across energy drink advertisements?
		TV commercials
		Online ads
		Print media
		Outdoor billboards
		Other

Packaging_preference: This column represents the response received for the below question.

	What type of packaging or bottle design would attract you to purchase an energy drink?
		Compact and portable cans
		Innovative bottle design
		Eco-friendly design
		Collectible packaging
		Other

Limited_edition_packaging: This column represents the response received for the below question.

	Would you be more likely to buy an energy drink with limited edition packaging?
		Yes
		No
		Not sure

Price_range: This column represents the response received for the below question.

	What price range do you consider reasonable for an energy drink?
		Below 50
		50-99
		100-150
		Above 150

Purchase_location: This column represents the response received for the below question.

	Where do you typically purchase energy drinks?
		Local stores
		Supermarkets
		Online retailers
		Gyms and fitness centers
		Other

Typical_consumption_situations:  This column represents the response received for the below question.

	In which situations or activities do you typically consume energy drinks?
		Sports/exercise
		Studying/working late
		Social outings/parties
		Driving/commuting
		Other 
## Key Insights
1. **Demographics**
   * Of the 10K respondents, 980 respondents have CodeX as their current energy drink brand.
   * 60% of the respondents were male while rest were either Female or Non binary.
   * Approximately 55% of the respondents are in the age group of 19-30 while only about 6.43% of the respondents are above the age of 46.
   * Approximately 65% of the respondents are from Bangalore, Hyderabad and Mumbai while just 1% from Lucknow.
   * Approximately 26% of all the respondents who have heard about CodeX as an energy drink are male while 18% are female.
2. **Consumer Preferences**
   * Approximately 30% of the respondents desired reduced sugar content in the energy drinks while about 25% of the respondents preferred more natural ingredients.
   * About 40% of the respondents preferred their energy drinks in compact and portable cans while about 30% desired for innovative bottle design.
   * Roughly 36% of the respondents consumed energy drinks for increased energy and focus while abot 24% consumed to combat fatigue.
   * Approximately 39% of the respondents had caffeine as their preferred ingredient.
   * Typical consumption situation for majority of the respondents was either during sports/exercise or while studying/working late.
   * 50 to 99 was the preferred price range for about 43% of the respondents while about 16% of the repondents were ready to pay even a price above 150.
3. **Competion Analysis**
   * Except Gangster all energy drinks have a better taste experience rating than CodeX.
   * Brand reputation and taste/flavor experience are the major reasons for choosing energy drinks brand.
   * Cola-Coka is the most popular brand, followed by Bepsi and Gangster, preferred by approximately 25% of the respondents.
4. **Marketing Channels**
   * Online ads is the most effective channel for reaching potential customers followed by TV Commercials.
   * Of all the respondents with current brand CodeX, who came across energy drinks through online advertisements, approximately 51% had heard about CodeX before, while in case of TV Commercials, only 33.33% of the respondents who came across energy drinks through TV Commercials, had heard about CodeX before. Online advertisements are therefore more effective in reaching CodeX customers.
5. **Brand Penetration**
   * Almost equal no. of CodeX respondents are from Tier I and Tier II cities.
   * General perception of energy drinks is that they are effective while a large proportion of the respondents consider energy drinks as dangerous.
   * Pune and Ahmedabad are the only cities where there are more respondents with a negative brand perception of CodeX as compared to the positive perception. Jaipur has the worst taste experience rating, while Lucknow has the best taste experience rating of 4, but the least number of respondents are from Lucknow, so definitely a potential for CodeX to tap.
   * Among the current consumers of CodeX, only in Delhi and Mumbai there were more respondents who had heard before about CodeX, while Delhi and Mumbai were the only cities where more respondents had not tried CodeX before as compared to those who had tried.
6. **Purchase Behavior**
   * Supermarkets and Online retailers are the most preferred locations for consumers to purchase energy drinks.
   * More than 65% of the respndents consume energy drinks to either stay awake during work/study or before exercise.
   * There is an almost equal no. of respondents who prefer limited edition packaging and those who do not.
   * Alost 50% of the respondents are interested in natural or organic ingredients in their energy drinks.
   * Energy drinks not being available locally and health concerns are the biggest reasons preventing respondents from trying energy drinks.
7. **Product Development**
   * The average taste experience rating of CodeX is 3.27 which is competitive with industry rating of 3.30, those in the age group of 31 to 45 have given the lowest rating of 3.21 while those in the age group of 46-65 have given the highest rating of 3.43.
   * Female have provided higher taste experience rating of 3.34 as compared to male rating of 3.24.
   * 50 to 150 is the preferred price range of almost 74% of the respondents.
   * More than 80% of the respondents have a positive or neutral perception of CodeX as a brand.

