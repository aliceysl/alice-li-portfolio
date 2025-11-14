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

<mark>**Insight 1:** Heatmaps are the clearest and most effective charts</mark>
- Both participants agreed heatmaps are the easiest to understand
- They enable quick comparison of brands and recall reasons

<mark>**Insight 2:** Sankey Diagrams Need Simplification</mark>
- Both agree Sankey diagrams are informative but high in noise
- Become messy when too many defect categories are present; require:
- Adding labels
- Using them as supplementary rather than primary visuals

<mark>**Insight 3**: Every chart requires a title and caption</mark>
- Users need guidance on “what question this chart is meant to answer”
- The title area and subtitle require reinforcement

## Step five: build the solution

_Include and describe your final solution here. It's also a good idea to summarize your thoughts on the process overall. When you're done with the assignment, this page should all the items mentioned in the assignment page on Canvas(a link or screenshot of the original data visualization, documentation explaining your process, a summary of your wireframes and user feedback, your final, redesigned data visualization, etc.)._

## References
_List any references you used here._

## AI acknowledgements
_If you used AI to help you complete this assignment (within the parameters of the instruction and course guidelines), detail your use of AI for this assignment here._

