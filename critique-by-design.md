| [Home Page](https://cmustudent.github.io/tswd-portfolio-templates/) | [Data Visualization Critique](DV-critique-1) | [Data visualization](DV-1) | [Critique by Design](critique-by-design) | [Final Project I](final-project-part-one) | [Final Project II](final-project-part-two) | [Final Project III](final-project-part-three) |

# 📘 Critique By Design - MakeoverMonday Redesign Project
## NHTSA Vehicle Recalls by Manufacturer
_By Alice Li
Carnegie Mellon University — Telling Stories with Data_

## Step one: the visualization

I selected the visualization **“NHTSA Recalls by Manufacturer”** from MakeoverMonday for redesign.
My reasons for choosing this topic are as follows:
- **High issue importance:** Vehicle recalls are directly linked to road safety.
- **Extensive data coverage:** NHTSA recall data spans over 50 years, from 1966 to 2023.
- **Difficulty comparing brands and defect categories:** While interactive, the original visualization confined information within pie charts.
- **Lack of timeline and contextual information:** Viewers may misunderstand, leading to brand bias or misconceptions.

My goal is to enable users with a single glance to understand:
- Time trends
- Defect types
- Differences between brands

## Step two: the critique
I analyzed the original visualization using Stephen Few's evaluation model, focusing on aspects such as “message clarity, comparative capability, design consistency, and authenticity.”

### What is the message?

This pie chart primarily shows:
- Which brand has the most recalls
- Clicking reveals the main defect types for that brand's recalls

In other words, it aims to convey both “overall comparison” and “defect classification.”

### Strengths

The interactive design guides users to explore defect classifications (by clicking brands), with colors enabling viewers to distinguish different brands. It effectively presents the theme of “comparing recall volumes.”

### Weaknesses

- Pie charts are unsuitable for comparing multiple brands: When the number of categories increases, differences become harder to discern, and excessive colors can lead to insufficient information density.
- Inability to compare defect types across brands: Pie charts limit presentation, allowing only a deep dive into all defect types for one brand at a time.
- Lacks temporal context: Despite covering 57 years of data, pie charts only show aggregate totals

### Potential Misinterpretation
**```Recall volume ≠ quality metric```**

Without total sales volume, market share, or vehicle count, viewers may mistakenly assume brands with higher numbers perform worse. The title and description also fail to clarify this.

> When redesigning, it's not just about “improving the chart,” but about clarifying:
> What information does the `audience` of this chart `need`? What questions do I want it to answer?

## Step three: Sketch a solution
Based on my critiques, I created three sketches addressing three points.

### 1️⃣ Line chart → Lack of trend visualization
- Show how recall volumes for each brand change over time
- Address the limitation of pie charts displaying only total figures

<img src="line chart - sketch.jpg" width="800">

### 2️⃣ Heatmap → Unable to compare recall reasons across brands
- At a glance, compare which brands most frequently exhibit issues with specific defects
- Users can compare without having to click through multiple pages

<img src="heatmap - sketch.jpg" width="800">

### 2️⃣ Sankey diagram → Lack of structural perspective
- Distribution of reasons for brand recall

<img src="Sankey diagram - sketch.jpg" width="800">

## Step four: Test the solution
- **Participant 1:** 25 years old, male, accounting background, no design background, basic knowledge of cars
- **Participant 2:** 30 years old, female, product designer, design background, unfamiliar with cars

### Questions & results

#### Overall understanding
- What do you think these three sketches are presenting?
- Which one is easiest to understand? Which one is hardest to understand? Why?

  - **Interview 1**
    - Heatmaps are the most intuitive and easiest to understand.
    - Sankey diagrams show brand recall volume, but their numerous branches can make them cluttered.
    - Line charts initially gave the impression that higher values were better (since “higher is better” is the common assumption).

  - **Interview 2**
    - Each chart should include a clear title and brief description.
    - Heatmaps are the most intuitive (especially when comparing multiple brands).
    - Sankey diagrams require closer reading to understand.

#### Line Chart
- What do you think this chart is talking about?
- Is it easy to understand? Any questions?
- What other information or labels would you like to see?

  - **Interview 1**
    - Not a big fan of line charts, but they're tolerable when paired with heatmaps.
    - Consider adding a note: “Higher values indicate more recalls, not necessarily better performance.”

  - **Interview 2**
    - I prefer line charts because they show trends over time rather than just total figures.
    - I recommend adding data limitation annotations (e.g., “no market share data available,” “does not indicate quality”).

#### Heatmap
- Are the heatmap's color gradients easy to understand?
- Can you quickly identify “the most common defects for a specific brand”?

  - **Interview 1**
    - Clearly distinguish between the brand and the reason for recall.
    - Color intensity allows people to immediately grasp the key points.

  - **Interview 2**
    - Color intensity is quite effective.
    - Sorting from dark to light would make it easier to understand.

#### Sankey Diagram
- Do the lines help you understand the flow direction?
- What do the lines make you feel?

  - **Interview 1**
    - Advantages: Provides insight into the general types of defects associated with each brand.
    - Disadvantages: Multiple lines can appear cluttered, making it less readable than a heatmap.

  - **Interview 2**
    - The concept is good, but the sketch lacks numerical labels, making it difficult to discern differences in magnitude.
    - If there are too many defect categories, consider simplifying them.

#### Improvements
- What order do you think these three images should be presented in?
- Which one is most helpful? Which one needs the most improvement?
- Is there any other information you feel is missing?

  - **Interview 1**
    - Recommended to include market share comparisons to avoid the misunderstanding that “more recalls = poor vehicle quality.”
    - Believe annotations should be added to prevent misunderstanding.

  - **Interview 2**
    - Figure captions, axis labels, and text within figures need to be clearer.
    - I believe the three figures could form a dashboard, ideally arranged in the logical sequence of “trends → comparisons → flow.”


### Synthesis: 

<mark>Insight 1: Heatmaps are the clearest and most effective charts</mark>
- Both participants agreed that heatmaps are the easiest to understand
- They enable quick comparison of brands and recall reasons

<mark>**Insight 2: ** Sankey Diagrams Need Simplification</mark>
- Both agree that Sankey diagrams are informative but high in noise
- Become messy when too many defect categories are present; require:
- Adding labels
- Using them as supplementary rather than primary visuals

<mark>Insight 3: Every chart requires a title and caption</mark>
- Users need guidance on “what question this chart is meant to answer”
- The title area and subtitle require reinforcement

## Step five: build the solution

_Include and describe your final solution here. It's also a good idea to summarize your thoughts on the process overall. When you're done with the assignment, this page should all the items mentioned in the assignment page on Canvas(a link or screenshot of the original data visualization, documentation explaining your process, a summary of your wireframes and user feedback, your final, redesigned data visualization, etc.)._

<div class='tableauPlaceholder' id='viz1763106827182' style='position: relative'><noscript><a href='#'><img alt='Line Chart ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ca&#47;CarsRecallTrend&#47;LineChart&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='CarsRecallTrend&#47;LineChart' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ca&#47;CarsRecallTrend&#47;LineChart&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='zh-TW' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1763106827182');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>


## References
- American Enterprise Institute. (2016). Animated chart: Market shares of U.S. auto sales, 1961–2016. Retrieved from https://www.aei.org/carpe-diem/
- Few, S. (2006). Data Visualization Effectiveness Profile. Perceptual Edge.
http://www.perceptualedge.com/articles/visual_business_intelligence/data_visualization_effectiveness_profile.pdf
- Garvey, B. Auto Fatalities Visualization Sketches. Retrieved from
http://plotdevice.bengarvey.com/auto
- Hint.fm. (2010). Design and Redesign. Retrieved from
https://medium.com/@hint_fm/design-and-redesign-4ab77206cf9
- MakeoverMonday. (2023). NHTSA Recalls by Manufacturer. Dataset and original visualization retrieved from
https://www.makeovermonday.co.uk/
- NHTSA. (2023). Vehicle Recall Data. National Highway Traffic Safety Administration.
https://www.nhtsa.gov/recalls
- Multiple Views – Visualization Research Explained. (n.d.). Data is Personal: What We Learned from 42 Interviews in Rural America.
https://medium.com/multiple-views-visualization-research-explained/data-is-personal-what-we-learned-from-42-interviews-in-rural-america-93539f25836d
- Riley, J. (2018). Correlation, Causation & Misleading Data Claims [Video].
YouTube. https://youtu.be/emb6EoIDcnw
- VizHealth. (n.d.). Visualizing Health Wizard.
http://www.vizhealth.org/wizard/
- Youtube – MakeoverMonday. (n.d.). Critique Videos & Watch Me Viz.
https://www.youtube.com/playlist?list=PLX-uPHRG0cLaArxVL-tz209lw3sJZDlNL

## AI acknowledgements
_In this assignment, I used Generative AI to assist with the following tasks:_

_- Understanding assignment instructions: Clarifying requirements for each step and confirming submission format specifications._
_- Refining textual expression: Assisting in adjusting the tone when describing critiques, insights, and user interview feedback to ensure clarity, conciseness, and fluency._

_All visual sketches, data analysis, user interviews, final decisions, and redesigns were completed by me personally._

