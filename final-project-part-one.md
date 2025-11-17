| [Home Page](https://aliceysl.github.io/alice-li-portfolio/) | [Data Visualization Critique](DV-critique-1) | [Data visualization](DV-1) | [Critique by Design](critique-by-design) | [Final Project I](final-project-part-one) | [Final Project II](final-project-part-two) | [Final Project III](final-project-part-three) |



# The Impact of Women's Educational Level in the United States on Family Composition and Life Choices
_By Alice Li Carnegie Mellon University — Telling Stories with Data_

# 1. Outline
 
This project focuses on how rising educational level of US women has transformed family structures—including marriage, divorce, childbearing, marital stability, and number of marriages—and how women are reprioritizing life goals in modern society.

While popular assumptions suggest “higher education → less likely to marry → fewer children,” such narratives oversimplify realities and overlook women's structural environments and developmental needs.

However, the data reveal a different narrative for highly educated women:
- Marrying later, yet having more stable marriages
- Having children later, yet investing greater time and resources in parenting
- Demonstrating stronger autonomy in partner selection and relationship quality

These trends are not because women reject family life, but because of:
- Increased career opportunities for women (higher salaries, promotions, etc.)
- Childcare costs, parenting expenses, and housing affordability severely impacting family formation
- Changes in how modern couples meet (online dating, workplaces, etc.)
- Women preferring to start families under more stable, secure, and resourceful circumstances

**Increased education for women = more life choices ≠ fewer families**

What truly shapes family structures is whether the environment and system support modern women's lifestyles and pursuits.

# 2. Project structure 

## (A) Changes in U.S. Family Composition
Purpose: To provide background context for audiences and dispel existing misconceptions.

- Marriage and Educational Level: Declining marriage rates, rising age at first marriage, delayed childbearing, and a decrease in divorce rates over the past decade (though varying by educational attainment)
- Regional Differences: Higher marriage rates in the Midwest and South, lower rates in the Northeast/West Coast

**While it may appear that “increased female educational attainment” drives these changes, the answer is more complex.**

_Resources: ACS、NCFMR_

## (B) How does educational level influence family formation?
- Higher education → Later marriage, later childbearing, more stable marriages (lower divorce rates)
- Lower education → Earlier marriage and childbearing, higher divorce rates
- State-level educational distribution correlates closely with marriage rates

_Data: ACS (EDUC × MAR × DIV), NSFG (AGEAT1STMARR, MARLENGTH)_

## (C) Female Education Improvement → Better Career Development, Not Rejecting Family
- Highly educated women earn more and hold higher positions
- Women's contribution to household income increases
- Higher-educated women pursue career development → Adjusting family formation timing
- Delaying marriage isn't about unwillingness to marry, but waiting for suitable conditions

_Sources: BLS Women’s Earnings, DOL Women’s Bureau, ACS Household Income_

## (D) Four systemic burdens better explain family delay than education:
- High childcare costs (the U.S. ranks among the most expensive in the OECD)
- High total child-rearing expenses (USDA data shows an average of $200,000–$300,000)
- High housing affordability challenges (price-to-income ratios of 5–10 times)
- Limited work flexibility (highly educated women rely more on career progression)

_Sources: OECD Childcare Costs, U.S. DOL Childcare Prices, USDA Child Costs, Harvard JCHS Housing Data, Zillow ZORI_

## (E) Education Empowers Women to Make Better Partner Choices
- Highly educated women have greater opportunities to meet partners through online dating or professional settings
- The timeframe from meeting to marriage varies by educational attainment
- Women prioritize partner quality and shared values over early marriage

_Source: HCMST (Stanford)_

### `This demonstrates that higher education is not the issue—the real question is whether the environment and systems support women.`

# 3. Initial sketches

[Drawing]

# 4. The data
| Name | URL | Description |
|------|------|-------------|
| **ACS PUMS – American Community Survey** | [Link 1](https://www.census.gov/programs-surveys/acs/microdata.html) <br> [Link 2](https://www2.census.gov/programs-surveys/acs/data/pums/) | Analyze the relationship between women's educational level and marriage rates, divorce rates, fertility rates, number of marriages, and regional variations. |
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
