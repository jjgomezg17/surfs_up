# surfs_up

## Overview of the analysis

### The purpose of this analysis is to study two months of temperature in particular, this to be able to propose to investors that the business can be profitable at different times of the year. By doing it with two months, you can compare the descriptive statistics of each case and draw conclusions about future studies and analysis models in particular for the business.

## Results

### June had 1700 temperature data analyzed with a mean of 74.94, a standard deviation of 3.25, with a minimum temperature of 64 and a maximum of 85.

### Meanwhile, December had 1517 temperature data analyzed with a mean of 71.04, a standard deviation of 3.74, with a minimum temperature of 56 and a maximum of 83.

img

img

### This may lead us to think that the month of June may be more accurate than December in measures of central tendency, seeing that June has about 200 more samples, however there is not enough statistical evidence to support this.

### On the other hand, it can be said that on average the temperatures of June are higher than those of December when observing that the average is higher for the month of June. What is equally evident when observing the minimum and maximum of June is higher than the month of December to the same extent as the average.

### When observing the percetiles, the same conclusions already mentioned are evident. Well, in the case of June, 75% of the data are below 77 and for December below 74. This leads to the conclusion that the month of June generally has higher temperatures than the month of December.

## Summary

### The differences between the month of June and December are not substantially significant to be able to argue that the proposed business could not be successful in the different seasons of the year. However, it is evident that the month of June does present temperatures higher than the month of December but not with changes that are abrupt enough to draw conclusions about the business itself. For now, with the data available, it could be said that a business like the one suggested would be successful in both seasons of the year, since no temperature is lower than one that in theory would not work for the proposed business idea.

### To obtain more information or more useful information for the month of June and December in the future, the following queries can be executed to obtain more conclusions in this regard.

### The following queries of code would describe the precipitation that occurred in these two months, which could bring more information when making decisions for the business, because by knowing this data, the climate that occurred in these months could be studied in more depth and learn how they differ and how they could affect or benefit the business.

#### june_prcp = session.query(Measurement.prcp).filter(extract('month', Measurement.date) == 6).all()
#### june_prcp_df = pd.DataFrame(june_prcp)
#### june_prcp_df.describe()

#### dec_prcp = session.query(Measurement.prcp).filter(extract('month', Measurement.date) == 12).all()
#### dec_prcp_df = pd.DataFrame(dec_prcp)
#### dec_prcp_df.describe()
