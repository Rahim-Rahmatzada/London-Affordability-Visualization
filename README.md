# London Housing Affordability Visualization

This project explores spatial and temporal variations in housing affordability across London using interactive, data-driven visualizations. It compares average house prices by buyer type (first-time vs. former owner-occupier) and purchase method (cash vs. mortgage) across boroughs, revealing trends in economic accessibility and neighbourhood transformation.

## Overview

This project aims to address the following key questions:
- How do spatial and temporal variations in housing affordability reveal patterns of economic accessibility?
- What differences can be seen between first-time buyers and former owner-occupiers?
- How do patterns of cash and mortgage purchases indicate neighbourhood transformation?

All visualizations are interactive and created using the Elm + VegaLite stack with publicly available datasets.

## Visualizations

### 1. **Borough Price Maps**
- Choropleth maps of average prices by borough for both first-time buyers and former owner-occupiers
- Month-by-month filter via interactive slider
- Region selector to highlight borough-specific data

### 2. **Price Trend Line Charts**
- Monthly price trend lines for all boroughs
- Highlighting of selected boroughs to analyze specific fluctuations
- Comparison of buyer types over time

### 3. **Stacked Area Charts**
- Proportional distribution of total housing prices by borough
- Compares market share between boroughs for each buyer type
- Tracks shifts across 2021

### 4. **Cash vs. Mortgage Purchase Maps**
- Grid-style maps with spatial layout of boroughs
- Average price and sales volume encoded through color and size
- Split view to compare cash and mortgage trends

### 5. **Sales Volume Heatmaps**
- Borough-wise monthly heatmaps of sales volume
- Reveals temporal peaks in buyer activity (e.g. around Stamp Duty Holiday)

## Quick Insights

- A strong west-east divide exists in affordability, with boroughs like Kensington and Westminster remaining unaffordable for first-time buyers, while Barking and Dagenham remains consistently accessible.
- Former owner-occupiers consistently purchase at higher price points and face greater price volatility, especially in high-end boroughs.
- The Stamp Duty Holiday caused significant spikes in prices and transactions, particularly in wealthier boroughs.
- Outer boroughs are dominated by mortgage buyers, indicating greater affordability and accessibility for financed buyers.
- Central boroughs are dominated by cash purchases, reflecting wealth concentration and investment-driven markets.


## Technologies Used

- [Elm](https://elm-lang.org/)
- [Elm-VegaLite](https://github.com/gicentre/elm-vegalite)
- [VegaLite](https://vega.github.io/vega-lite/)
- [Topological GeoJSON](https://gicentre.github.io/data/geoTutorials/londonBoroughs.json)
- CSV Data from London Housing Sales and Land Registry

## Getting Started

Clone the repo and run your Elm environment with the VegaLite and Tidy libraries. All data is fetched from public URLs and no authentication is required.

```bash
git clone https://github.com/Rahim-Rahmatzada/London-Affordability-Visualization.git
cd London-Affordability-Visualization
elm reactor
```

![](Images/image1.png)
![](Images/image2.png)
![](Images/image3.png)
![](Images/image4.png)

## Full Insights

1. West-East divide and price dynamics
2. Market distribution and buyer type impact
3. Economic accessibility and neighborhood segmentation

**Spatial and temporal variations revealing patterns in housing affordability**

The first visualisation of housing prices across London boroughs in **2021** show sharp variation both spatially and temporally, indicative of stark patterns of economic accessibility. Among many interesting observations, what immediately comes into view is the persistent west-east divide of affordability. For example, central-western boroughs like **Westminster, Kensington and Chelsea**, and **Hammersmith** and **Fulham** have always had consistently high prices within a bracket for housing accommodations, taking in a predominantly high-end clientele. For **Kensington and Chelsea**, the prices were between **£1,041,764** and **£1,317,701** for first-time buyers, while for former owner-occupiers, the prices were between **£1,366,940** and **£1,755,585**.

However, the house prices in the outer eastern boroughs such as **Barking and Dagenham** as well as **Bexley**, are relatively affordable. House prices for **Barking and Dagenham** for first-time buyers were between **£287,962 and £299,390**, thus being one of the most economical cities.
That really points to entrenched economic disparities in London, with its western and central parts remaining powerful enclaves of money and prosperity. Again, this report shows that those eastern boroughs have provided a stable lead on house affordability and are really the key areas where economic access is guaranteed, more for first-time buyers and groups with low income. This also extends the affordability factor since the price trend volatility remains comparatively less in eastern boroughs than in central areas, where prices jump up and down very fast, creating barriers to entry.

**First-Time Buyers vs. Former Owner-Occupiers**

There is a clear distinction in price affordability and behaviour within first-time buyers compared to former owner-occupiers. In nearly all the boroughs, former owner-occupiers have a much higher average prices compared to first-time purchasers. This fact reflects the investment in high-valued properties made possible by their acquired equity and financial capacity. For example, in **Westminster**, while former owner-occupiers paid prices ranging between **£979,800** to **£1,221,668**, for first-time buyers, the prices vary from **£828,041** to **£1,018,702**. This price differential puts into perspective how challenging it is to become a first-time buyer, especially in upper-class boroughs where accessibility is even harder.

Meanwhile, for less expensive boroughs such as **Barking and Dagenham**, the difference is much smaller, at **£299,390** to **£287,962** for first-time buyers and from **£329,134** to **£344,384** for former owner-occupiers, which means outer boroughs remain accessible for more buyers. The other observations presented in the visualisation are that former owner-occupiers face much greater price volatility, especially at the centre, this is because they participate in more volatile and competitive property markets.

**West-East Divide and Price Dynamics**

Moving on, by taking a deeper analysis into the visualisations we can reveal a clear west east divide and how prices differentiate for these areas. The maps and corresponding line charts show residential property prices are unusually high in western and central boroughs but also extremely volatile. This becomes extremely clear for boroughs such as **Westminster and Kensington** and **Chelsea**, where the month-on-month change in house prices is sometimes over **£200,000**. These variations seen around the stamp duty holiday deadline being in **July** help further illustrate how responsive such high value markets can be to fiscal policy and economic incentive and how these policies can increase the existing disparities by even more .

Contrastingly, the relatively stable trends in the east such as in **Barking and Dagenham** and **Bexley** reflect their stability and resilience even throughout the stamp duty period from January to the end of June. These areas present significantly smaller deviations in monthly prices, often staying below **£50,000**, thereby making them more predictable and accessible to prospective buyers. Additionally, the trend in the graph shows that house prices in the different boroughs peaked during months **7** and **8**. This coincides with the end of the Stamp Duty Holiday, which caused a surge in market activity. The common response from all boroughs indicates that changes in policy can have a huge but somewhat unpredictable impact on housing markets, making various regions even more unequal.

**Market Distribution and dominance by boroughs**
The stacked area visualisation highlights the proportional contributions of each borough to total housing prices for first-time buyers and former owner-occupiers across London during 2021. These charts show the distribution of housing prices as a percentage of the total for each buyer type, summing to 100% for every month by normalising the data from integer values into percentages helping the user to also read the data more easily. Essentially allowing us to identify which boroughs dominate the market and how contributions vary between first-time buyers and former owner-occupiers over time.

Such central boroughs such as **Kensington and Chelsea**, **City of Westminster**, and **City of London** always top in the housing market for both types of buyers. In **January**, **Kensington and Chelsea** contributed about **7.3%** of the total housing price for first-time buyers and an even higher **7.5%** for former owner-occupiers, proving the consistent appeal it has among high-income buyers. Similarly, the **City of Westminster** contributed about **5.3%** for first-time buyers and **5.0%** for former owner-occupiers in the same period. These boroughs are, in their nature and global prestige of luxury properties, often hotbeds for high-value transactions irrespective of the buyer type.

In stark contrast, outer boroughs like **Barking and Dagenham** and **Bexley** present much smaller shares-a fact that indicates their affordability. Take, for instance, **Barking and Dagenham** at just about **1.8%** for first-time buyers and **1.6%** for former owner-occupiers in January. This borough is an area of convenience for buyers looking to seek lower-priced houses, particularly for first-time buyers.

This basically means that, over the year 2021, little variation was seen in the proportion contributed by each borough, with the central boroughs-like **Kensington and Chelsea** and **Westminster** always at the top because of continuous demand in those areas, and outer ones such as **Barking and Dagenham** and **Havering** steadily contributing a minimal amount; it reflects the predictability of these markets through such stability.

Proportional stability across most boroughs would suggest a segmented market in which the richest areas retain high-value transactions and the outer boroughs are used as more accessible entry points for lower-income buyers. It would appear that the above visualisations do not really indicate extreme shifts of dominance across boroughs; however, fiscal policies such as the Stamp Duty Holiday have further increased activity across already high-value areas.

**Spatial and temporal trends in Cash vs. Mortgage Purchases**
The grid map presents a clear spatial divergence in cash and mortgage purchases throughout 2021. Cash purchases are dominated by more central boroughs like **Kensington and Chelsea**, along with the **City of Westminster**, reflecting their appeal to rich buyers and investors who can afford average house prices of more than **£1.2M**. Whereas, greater volumes of mortgage transactions occur in outer boroughs like **Bromley** and **Havering** at much lower average prices of around **£467K** and **£384K** respectively. These are the key entry points for financed buyers, such as first time buyers and families .

By further analysing the heat map, different temporal trends are clear, in particular, for mortgage purchases. An extraordinary surge in mortgage sales volume was evident in **June and July of 2021** because of the Stamp Duty Holiday deadline. Such a policy encourages buyers to accelerate their purchases, especially in high-value boroughs like the **City of Westminster** and **Kensington and Chelsea**, where the likely tax gains were very high. On the other hand, cash purchases remained consistent throughout the year since they are independent of these kinds of fiscal incentives.

These patterns reveal the neighbourhood transformations even when we are limited to one year’s worth of data, as outer boroughs increasingly accommodate funded buyers in search of more affordable and accessible options. Dependence on mortgages in boroughs like **Croydon** and **Havering** underlines their role within a growing supply of housing to London's wider population. Yet the predominance of cash buying in inner boroughs underlines their exclusivity, catering to established wealth and international capital. This dual nature of purchase dynamics reinforces the economic segmentation of London's housing market in a manner that accessibility and wealth concentration describe different buyer behaviours.

## Design Justification

1. Colour Encoding
2. Interactivity
3. Layout

**Colour Encoding**
One of the most important features of these visualisations is colour encoding; complex data intuitively and accessibly delivered. Diverging colour schemes displaying borough-level housing prices such as the Viridis scheme help in following **Tufte's** principle of clarity and lack of clutter in visualizations. These colour schemes would serve to make the quantitative variations in average housing prices clearly visible, ranging from lighter to darker tones, indicating lower to higher prices. The reader would easily reach out to the borough with housing prices falling into either the cheaper or more expensive bracket as this gradient makes it more expressively comprehensible. This would, therefore, comply with **Munzner's** principle "expressiveness" where the visual marks should express precisely their respective data. Moreover, consistency in colour scales across buyer types-first-time buyers and former owner-occupiers-allows for direct comparison. It permits intuitive exploration of spatial disparities and price trends without any mental effort needed for adapting to a different meaning of colours. Such consistency is very relevant to **Wilkinson's** Grammar of Graphics, where emphasis is placed on consistency of variable encoding.

This falls in line with **Bertin's** foundational work in visual semiology, wherein he provides that color should be used systematically to represent variation in data in a manner that agrees with the human perception; this is its most powerful application. In applying the Viridis colour scheme, I follow the suggestions of Bertin to vary in value that is, lightness-being naturally ordinal, intuitively conveying the variation in price across boroughs to the viewer.

Additionally, accessibility was also a key aspect I took into mind when creating my visualisations. The palette Viridis has also been chosen because it is perceptually uniform and suitable for colour vision deficiencies, which allows for inclusivity of the wide audience without differential access. This approach lets the most basic feeling of inclusive design get through: making sure users-independence of their ability to see and interpret the data correctly. Carefully chosen colour schemes, their consistent use, and consideration for accessibility make the visualization insightful yet correctly execute the best practices in data visualization.

**Interactivity**
Interactivity adds to these visualisations in terms of both usability and depth, letting users interactively delve into the data and focus on their specific interests. It generally follows the guiding principle outlined in **Shneiderman's** framework: "Overview first, zoom and filter, then details-on-demand". Users are able to filter the data temporally using a month slider to explore the trend for the whole year of 2021. This helps as a great tool to analyse temporal patterns for example monitoring how house prices change because of other external causes over time. It also enables selection among boroughs which when clicked highlight the corresponding borough's line within the line chart, hence the ability to go deep into both the spatial and temporal patterns in significantly greater detail. By integrating these tools, the visualization does both: exploration and analysis; hence, supporting **Munzner's** "analysis" and "explore" goals.

Other important interactive visual means are the tooltips with information on average price, name of boroughs, and other relevant measures. Such details are embedded right within the visualization itself without making the user refer elsewhere to gather the information. This is what constitutes an excellent user experience. The inclusion of tooltips attempts to follow the principle of the low interaction cost, where the user gets more detailed information with little effort. Again, annotating some of these, like Stamp Duty Holiday, really enhances the storytelling capability of relating the observed pattern in the data to an actual event. The contextualization builds on the feature that makes the user more insightful from the data while showing its capacity for both explanatory and exploratory ends.

Lastly, the interactive elements also adhere to **Heer and Shneiderman's** framework for visual analysis, especially their focus on view manipulation and coordination. Their work indicates that an effective interactive visualization should allow both data and view specification, which in my implementation has been achieved by introducing temporal filtering and the selection of boroughs. The tooltips and the synchronized views in this regard demonstrate typical examples of what Heer and Shneiderman referred to as "coordinate multiple views" so that a user can compare the relationships among various facets from the housing market dataset.

**Layout**
The charts are laid out to optimise readability, become more comparable, and to allow for both spatial and temporal analysis per Tufte's principles of maximizing the data to ink ratio. Generally, the structure of this overall dashboard is split into spatial mappings and temporal trends. By doing so, one can get an overall view of the pattern in the boroughs through the map view and then study the detailed temporal dynamics through line and area charts. The maps reveal a clear spatial presentation of housing prices, whereas the temporal charts reveal the series of prices for first-time buyers and former owner-occupiers. Combining these two sets of views enables the user to analyse both spatial and temporal dimensions comprehensively; hence, it will satisfy the **Shneiderman** principle of overview first.

Comparative analysis is further supported by the side by side arrangement of the visualizations as seen in the first graph. First-time buyer maps are placed beside those from former owner-occupiers, as are their respective temporal line charts. This helps to make the data comparable directly, and hence any disparities or commonalities between the buyer types shown. Furthermore, in the next visualisation of the cash versus mortgage purchases utilizing grid and heat maps, we balance the geographic reference with the simplicity of display by placing boroughs in a quasi-geographic layout becoming informative but not cluttered. This is an important design decision which maintains spatial relationships without clutter in the visual landscape faced by the users. This grid map was taken from the lecture notes from week 8 and adapted to my use case as I incorporated spatial and temporal patterns into the map.

Additionally, I reduce clutter and minimise unnecessary redundancy by streamlining legends and axes and in some cases even simply removing them. This is because shared colour scales and axis labels reduce intellectual strain to let the user focus on the data at hand, not the mechanics of the visualisation. If employed, legends are placed in a way to provide context to the data without disrupting the flow of data across the visualization. This follows **Munzner's** principle of "efficiency" and **Tufte's** emphasis on the removal of non-essentials in order to give real estate to the data. It, therefore, encapsulates the spatial, temporal, and comparative features into one, providing a comprehensive, logical, and persuasive pattern for analysing house price patterns in London.

## References

**Bertin, J.** (2011) Semiology of Graphics: Diagrams, Networks, Maps. Redlands, Calif.: Esri Press.

**Census Data** (2021) [UK House Price Index](landregistry.data.gov.uk).

**Heer, J., & Shneiderman, B.** (2012) [Interactive Dynamics for Visual Analysis](https://dl.acm.org/doi/10.1145/2133416.2146416), Communications of the ACM.

**Munzner, T.** (2014). Visualization analysis and design. AK Peters/CRC Press.

**Shneiderman, B.** (1996) [The eyes have it: A task by data type taxonomy for information visualization](https://drum.lib.umd.edu/bitstream/handle/1903/5784/TR_96-66.pdf), _Proceedings of the IEEE Symposium on Visual Languages_, pp.336-343.

**Stone, M.** (2006). Choosing colors for data visualization. Business Intelligence Network, 2.

**Tufte, E.** (2001) [The Visual Display of Quantitative Information](https://go.exlibris.link/HRpwwyBl), Graphics Press.

**Ware, C.** (2012) [Information Visualization: Perception for Design](https://go.exlibris.link/DpRlDxl8). S.L.: Morgan Kaufmann, ISBN: 9780128128763

**Wilkinson, L.** (2010b) [The Grammar of Graphics](https://go.exlibris.link/Y2gQqNZG). Springer, ISBN: 978 0387 24544 7

**Kachkaev, A et al** (2024) [London Boroughs Map](https://gicentre.github.io/data/geoTutorials/londonBoroughs.json)

**Kachkaev, A et al** (2024) [London Centroids And Grid Map](https://gicentre.github.io/data/geoTutorials/londonCentroidsAndGrid.csv)

