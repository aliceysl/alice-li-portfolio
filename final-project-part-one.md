| [Home Page](https://aliceysl.github.io/alice-li-portfolio/) | [Critique by Design](critique-by-design.md) | [Final Project I](final-project-part-one.md) | [Final Project II](final-project-part-two.md) | [Final Project III](final-project-part-three.md) |

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

<img src="gas sketch -2.jpg" width="800">

<img src="gas sketch -1.jpg" width="800">

# 4. The data

| Name                              | Link                                    | Description                                                                          |
|-----------------------------------|-----------------------------------------|--------------------------------------------------------------------------------------|
| TOP TIER Brand List               | https://toptiergas.com/licensed-brands/ | Determining whether a gas station is high-quality                                     |
| Google Places API                 | https://developers.google.com/maps      | Get the gas station location, brand, and coordinates                                 |
| ACS Income                        | https://data.census.gov                 | Analyzing Community Income and Differences in Oil Quality and Prices                 |
| Zillow ZHVI                       | https://www.zillow.com/research/data/   | Housing Prices vs. Gasoline Affordability                                            |
| WPRDC Crime                       | https://data.wprdc.org                  | Analysis of security and gas station distribution                                    |
| NCES / PA Department of Education | https://nces.ed.gov                     | Creating School Quality Indicators                                                   |
| EIA / AAA Oil Price Data          | https://www.eia.gov/petroleum/gasdiesel/ | Used as a benchmark for fuel price comparisons and cost-effectiveness calculations   |

# 5. Method and medium

This project will use Tableau to create primary charts and Shorthand to build an interactive long-form storytelling website. Gas station location data will be obtained via the Google Maps Places API, with Python used for data cleaning and spatial mapping. All final data and drafts (sketches) will be uploaded to GitHub, and Shorthand will present the final output by embedding Tableau charts.

## References

- TOP TIER. (n.d.). _Licensed brands_. https://toptiergas.com/licensed-brands/
- U.S. Census Bureau. (n.d.). _American Community Survey (ACS) 5-Year Estimates_. https://data.census.gov/
- Zillow Research. (n.d.). _Zillow Home Value Index (ZHVI)_. https://www.zillow.com/research/data/
- Western Pennsylvania Regional Data Center. (n.d.). _Crime data collections_. https://data.wprdc.org/
- National Center for Education Statistics. (n.d.). _Common Core of Data (CCD)_. https://nces.ed.gov/ccd/
- Pennsylvania Department of Education. (n.d.). _School performance profiles and assessment data_. https://www.education.pa.gov/
- American Automobile Association. (n.d.). _AAA Gas Prices_. https://gasprices.aaa.com/
- U.S. Energy Information Administration. (n.d.). _Gasoline and diesel fuel update_. https://www.eia.gov/petroleum/gasdiesel/

## AI Acknowledgements
I use generative AI to assist with:
- Understanding and confirming assignment instructions and formatting requirements
- Data research and document organization

I use grammar tools for:
- Draft refinement and tone adjustment

All analysis, visualization, and interpretation are completed personally by me.
