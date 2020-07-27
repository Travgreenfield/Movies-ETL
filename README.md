# Movies-ETL

## Assumptions

### Continued Data Structure Consistency

As we saw in the weekly lesson, the formatting for wiki data can change year over year. If the data pulled is consistently updated, the various 'pathing' to preferred JSON information may need to be widened or updated as well.

### Consistency in the Amount of Outliers

As is, outlier formatting for budget / box office (see Norwegian krone e.g.) are filtered out by default due to the fact that there were relatively little. If that grows, the integrity of the overall data maybe affected if those are continued to be automatically filtered out.

### All 3 Databases are Updated Consistently

Relying on 3 different sources for this data may mean that the quality will deteriorate over time if one is updated less frequently than the other 2.

### The Types of Movies Stays Consistent

In our current model, more less accessible moves (indies, foreign films, etc.) are more likely to be dropped due to the lack of budget and box office information. If the percentage of those types of movies grows in our dataset, we may be able to convert a lower percentage of data into useful information.

### Accessibility to the Data

Relying on third party organizations like Wikipedia assumes a consistent structure updating their information and a business model that makes it available for public consumption. 
