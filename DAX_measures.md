# Marketing Channels and Age Group count
chnl_age_count = 
SUMX(
    SUMMARIZE(
        fact_city_respondent_survey_response,
        fact_city_respondent_survey_response[Marketing_channels],
        fact_city_respondent_survey_response[Age]
    ),
    [number of respondents]
)

# city and brand_perception count
city_brand_perception = 
SUMX(
    SUMMARIZE(
        fact_city_respondent_survey_response,
        fact_city_respondent_survey_response[Brand_perception],
        fact_city_respondent_survey_response[City]
    ),
    [number of respondents]
)

# city and heard before count
city_heard_before_count = 
SUMX(
    SUMMARIZE(
        fact_city_respondent_survey_response,
        fact_city_respondent_survey_response[Heard_before],
        fact_city_respondent_survey_response[City]
    ),
    [number of respondents]
)

# brand perception and current brands count
codex_brand_perception_cnt = 
SUMX(
    SUMMARIZE(
        fact_city_respondent_survey_response,
        fact_city_respondent_survey_response[Brand_perception],
        fact_city_respondent_survey_response[Current_brands]
    ),
    [number of respondents]
)

# codex rating
codex_rating = 
CALCULATE(
    AVERAGE(fact_city_respondent_survey_response[Taste_experience]),
    fact_city_respondent_survey_response[Current_brands] = "CodeX")

# reasons for choosing brands and current brands count
codex_reasons_choosing_cnt = 
SUMX(
    SUMMARIZE(
        fact_city_respondent_survey_response,
        fact_city_respondent_survey_response[Reasons_for_choosing_brands],
        fact_city_respondent_survey_response[Current_brands]
    ),
    [number of respondents]
)

# industry rating
industry_rating = 
AVERAGE(fact_city_respondent_survey_response[Taste_experience])

# market channel and current brand count
mkt_chnl_brand_cnt = 
SUMX(
    SUMMARIZE(
        fact_city_respondent_survey_response,
        fact_city_respondent_survey_response[Marketing_channels],
        fact_city_respondent_survey_response[Current_brands]
    ),
    [number of respondents]
)

# preferred ingredients
preferred_ingredients = 
var VisibleGroups = DISTINCT(fact_city_respondent_survey_response[Ingredients_expected])
var result =
    CALCULATE(
        COUNTROWS(fact_city_respondent_survey_response),
        VisibleGroups,
        ALLSELECTED(fact_city_respondent_survey_response)
    )
return
    result

# CodeX and marketing channels count
SelectedBrandCustomerReachCount = 
COUNTROWS(
    FILTER(
        SUMMARIZE(
            fact_survey_responses,
            fact_survey_responses[Current_brands],
            fact_survey_responses[Marketing_channels]
        ),
        fact_survey_responses[Current_brands] = "CodeX"
    )
)

# Count of respondents interested in natural or organic ingredients
YesCount = COUNTROWS(FILTER(fact_city_respondent_survey_response, fact_city_respondent_survey_response[Interest_in_natural_or_organic] = "Yes"))