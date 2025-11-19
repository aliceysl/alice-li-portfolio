| [Home Page](https://aliceysl.github.io/alice-li-portfolio/) | [Data Visualization Critique](DV-critique-1.md) | [Data visualization](DV-1.md) | [Critique by Design](critique-by-design.md) | [Final Project I](final-project-part-one.md) | [Final Project II](final-project-part-two.md) | [Final Project III](final-project-part-three.md) |




# What does the gas station map tell us? Analyzing community differences in Allegheny County
_By Alice Li Carnegie Mellon University — Telling Stories with Data_

# 1. Outline
 
Daily commutes rely on gasoline, and the distribution of different fuel brands and gas stations is often regarded as “invisible infrastructure.” In Allegheny County—a region characterized by distinct local variations (where urban areas, affluent suburbs, industrial zones, and low-income communities coexist)—fuel quality, price disparities, and the geographic distribution of gas stations may reflect deeper socioeconomic structures.

This special feature aims to explore specific questions through data analysis: “Where are people more likely to access high-quality fuel?” “Do high-income vs. low-income neighborhoods have different fueling environments?” “Are fuel prices correlated with housing costs, public safety, or school quality?”

This project will use TOP TIER certification as an indicator of fuel quality, integrating multiple data sources including gas station locations, Census income data, Zillow housing prices, county crime statistics, and school quality metrics. Through maps, charts, and comparative indicators, I aim to construct a “fuel quality × community conditions” landscape narrative, revealing resource accessibility, consumer affordability, and potential inequalities within Allegheny County.

# 2. Project structure 

## Act I | Why Fuel Quality Matters?

- Introduction to TOP TIER certification: Representing the gold standard for fuel cleanliness and additive performance.
- Explaining Allegheny County's diverse composition: Pittsburgh's urban core, affluent suburbs, industrial towns, low-income communities, and more.
- Setting the stage for the central question: Is fuel quality linked to community disparities?

## Act II | Mapping the Fuel Landscape

- Use the Google Maps Places API to obtain all gas station locations and brands.
- Categorize brands into “TOP TIER” and “non-TOP TIER”.
- Visualize on a map: Where are high-quality gas stations concentrated? Where are the gaps (fuel deserts)?

## Act III | Adding Socioeconomic Layers

Perform spatial comparisons of gas station data with the following datasets:
- Income: Census ACS tract-level
- Housing Value: Zillow ZHVI
- Crime Rate: Allegheny County and Pittsburgh open data
- School Quality Proxy: NCES + PA Education indicators

Explore:
- Which areas are more likely to have TOP TIER stations?
- Do higher-priced suburbs vs. industrial towns exhibit different gas station characteristics?
- Do communities with better education and safety also have higher fuel quality?

## Act IV | Value for Money

Define the “fuel value for money” metric, which may utilize:
1. Fuel Value Index = Regional Average Fuel Price ÷ Fuel Quality Indicator (1 or 0)
2. Compare each community's fuel prices against the county average.

Explore:
- Which communities get more “value” for every dollar spent?
- Do low-income communities pay more for lower-quality fuel?

## Act V | Conclusion & Implications

-  Allegheny County's disparities and inequalities in fuel accessibility.
-  Discussion of potential impacts on commuting burdens, transportation behaviors, and community resource distribution.
-  Connections to broader social issues: the relationship between infrastructure and social class.

# 3. Initial sketches

[Drawing]

# 4. The data


| Name | URL | Description |
|------|------|-------------|
| **ACS PUMS – American Community Survey** | [Link 1](https://www.census.gov/programs-surveys/acs/microdata.html) · [Link 2](https://www2.census.gov/programs-surveys/acs/data/pums/) | Analyze the relationship between women's educational level and marriage rates, divorce rates, fertility rates, number of marriages, and regional variations. |
| **NSFG – National Survey of Family Growth** | [Link](https://www.cdc.gov/nchs/nsfg/nsfg6a.htm) | Analyze how the age at first marriage, duration of marriage, age at first childbirth, and educational level influence family formation tracks. |
| **NCFMR – Marriage & Divorce Rates** | [Link](https://www.bgsu.edu/ncfmr.html) | Presenting the long-term trends in national marriage and divorce rates as the context and opening of the story. |
| **HCMST – How Couples Meet and Stay Together** | [Link](https://data.stanford.edu/hcmst) | Analyze how women with different levels of education perceive their partners and how long it takes them to marry after meeting them. |
| **BLS – Highlights of Women’s Earnings** | [Link](https://www.bls.gov/opub/reports/womens-earnings/2023/home.htm) | Analyze differences in women's educational level, salary, job type, and career development. |
| **DOL Women’s Bureau – Earnings by Education & Sex** | [Link](https://www.dol.gov/agencies/wb/data/earnings/Median-weekly-earnings-educational-sex) | Compare the salaries of women with different levels of education and link them to household income. |
| **OECD – Net Childcare Costs Dataset** | [Link](https://stats.oecd.org/Index.aspx?DataSetCode=ELFS_CHILD) | Comparing childcare cost burdens between the United States and OECD countries, this analysis explains how systemic differences impact fertility and family formation. |
| **NDCP – National Database of Childcare Prices** | [Link](https://www.dol.gov/agencies/wb/topics/childcare) | Display childcare costs and their proportion of household income across U.S. counties, creating a childcare cost map for regional comparison. |
| **USDA – Cost of Raising a Child** | [Link](https://www.ers.usda.gov/data-products/cost-of-raising-a-child/) | Estimate the total cost of raising a child from infancy to adulthood and compare it to household income. |
| **Harvard JCHS – Housing Affordability Data** | [Link](https://www.jchs.harvard.edu/research/harvard-housing-data) | Analyzing the housing price-to-income ratio and the gender pay gap across states to explore the relationship between housing affordability and family formation. |
| **Zillow – Zillow Observed Rent Index (ZORI)** | [Link](https://www.zillow.com/research/data/) | Presenting urban rental affordability and supplementing home price affordability to form a comprehensive housing affordability analysis. |
| **Census – Income in the United States 2024** | [Link](https://www.census.gov/library/publications/2025/demo/p60-286.html) | Analyze household income structures, women's income contributions within families, and how income levels influence family composition. |




# 5. Method and medium
This project will use:

## (1) Tableau
- Create all primary charts (Bar, Line, Scatter, Map, Sankey, etc.)
- Combine with Shorthand or GitHub Pages to present interactive storytelling

## (2) Shorthand (or GitHub Pages)
- Build the interactive visual narrative pages for the final story
- Embed charts and present the Story Arc through segmented chapters

## (3) Python / Excel (Data Cleaning)
- Convert NSFG (Stata/SAS) data to CSV
- Cleanse large-scale ACS PUMS datasets

## References
### Family Composition, Marriage, and Fertility
- U.S. Census Bureau. (2024). _American Community Survey Public Use Microdata Sample (PUMS)_. https://www.census.gov/programs-surveys/acs/microdata.html
- Centers for Disease Control and Prevention. (2023). _National Survey of Family Growth_. https://www.cdc.gov/nchs/nsfg/index.htm
- National Center for Family & Marriage Research. (2023). _U.S. Marriage & Divorce Rates_. Bowling Green State University. https://www.bgsu.edu/ncfmr.html
### Couple Formation
- Rosenfeld, M. J., & Thomas, R. J. (Stanford University). (2023). _How Couples Meet and Stay Together (HCMST) Study_. https://data.stanford.edu/hcmst
### Women's Salaries and Workforce Participation
- U.S. Bureau of Labor Statistics. (2023). _Highlights of Women’s Earnings_. https://www.bls.gov/opub/reports/womens-earnings/2023/home.htm
- U.S. Department of Labor, Women’s Bureau. (2023). _Median Weekly Earnings by Educational Attainment and Sex_. https://www.dol.gov/agencies/wb/data/earnings/Median-weekly-earnings-educational-sex
### Childcare Costs and Parenting Burden
- Organisation for Economic Co-operation and Development. (2024). _Net Childcare Costs Dataset_. https://stats.oecd.org/Index.aspx?DataSetCode=ELFS_CHILD
- U.S. Department of Labor, Women’s Bureau. (2023). _National Database of Childcare Prices_. https://www.dol.gov/agencies/wb/topics/childcare
- United States Department of Agriculture, Economic Research Service. (2022). _Expenditures on Children by Families_. https://www.ers.usda.gov/data-products/cost-of-raising-a-child/
### Housing Affordability
- Harvard Joint Center for Housing Studies. (2024). _State of the Nation’s Housing: Data Downloads_. https://www.jchs.harvard.edu/research/harvard-housing-data
- Zillow Research. (2024). _Zillow Observed Rent Index (ZORI)_. https://www.zillow.com/research/data/
### Household Income
- U.S. Census Bureau. (2024). _Income in the United States: 2024_. https://www.census.gov/library/publications/2025/demo/p60-286.html

## AI Acknowledgements
I use generative AI to assist with:
- Understanding and confirming assignment instructions and formatting requirements
- Data research and document organization

I use grammar tools for:
- Draft refinement and tone adjustment

All analysis, visualization, and interpretation are completed personally by me.
