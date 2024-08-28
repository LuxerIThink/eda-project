# Exploratory Data Analysis Project

## Target

### I Phase - exploration and factors analysis
- Check chosen factors on customers quantity and cart value
  - Store type
  - School-free days
  - Special Offer
  - Work days and week days
  - Month splitted by 3 parts
  - Month splitted by weeks
  - Weather
  - Seasons
  - Months
  - States
  - States position
  - Others
- Use regression from ols model and A/B test.
- You can use unsupervised learning for searching focus groups
- Try to define what are types of shops (a, b, c, d)

### II Phase - prediction
- check factors influence on sales
  - regression
  - A/B tests
- Try to propose a method of analysis that will allow us to determine what store types a, b, c, d might mean.

#### Part I
- build model for every day of week decoupled from season and global factors
- find anomalies and their causes

#### Part II
- estimate mean sales for next 8 weeks (June and July) based on data to May 2015.
- designate model to data matching error

## What was made?
*This is only summary. Full description in notebook*

#### Phase I
- Functions for generic operations
- Heatmap of greater part of data was created
- Influence on sales, customers quantity and cart value was checked on factors like:
  - store type
  - assortment
  - special offer
  - school-free days
  - days of the week
  - month phase
  - weather
    - storm
    - rain
    - thunderstorm
    - fog
    - hail
  - months
  - states
- also was checked dependence between:
  - store types and assortment
  - hail and assortment
  - states and store types
  - states and assortment
  - states and school-free days

#### Phase II
- Depending on sales, factors such as store type, assortment, promotion, phase of the month, month, hail, day of the week were used.
- Sales prediction with 0.769 R-Squared mapping compared to real data on whole time range.
- Sales prediction with 0.999 R-Squared mapping compared to real data on next 6 month.
- Adding the State/StateName factor significantly reduces the result value.