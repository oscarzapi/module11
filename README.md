# module11
Github repository showcasing the results of the module 11.


Now that we've settled on our models and findings, it is time to deliver the information to the client. You should organize your work as a basic report that details your primary findings. Keep in mind that your audience is a group of used car dealers interested in fine-tuning their inventory.

Main takeaways from the previous analysis are: Price Distribution by Category

**Condition vs. Price**:

New vehicles have the highest median price and a wide range. Like new and excellent conditions also show higher prices than good or fair, which have lower medians and tighter spreads. Price clearly correlates with condition quality.

**Cylinders vs. Price**:

8-cylinder vehicles tend to have higher prices than 6 and 4-cylinder ones. This may reflect performance or luxury vehicle categories. Fuel vs. Price:

Electric vehicles show the highest price range, though they are few in number. Hybrid vehicles are priced higher than gas, which dominate the dataset but have lower median prices.

**Title Status vs. Price**:

Clean title vehicles have the highest and most stable price distribution. Rebuilt and salvage titles show significantly lower prices, likely due to perceived risk or damage history.

**Transmission vs. Price**:

Automatic vehicles have a higher median price than manual ones. This aligns with broader market preferences and vehicle types.

**Drive vs. Price**:

AWD (all-wheel drive) vehicles show the highest prices, though they are rare. RWD and FWD have similar distributions, with RWD slightly higher.

**Size vs. Price**:

Full-size vehicles have the highest price range and median. Mid-size and compact-size vehicles are priced lower, reflecting their market segment.

**Paint Color vs. Price**:

Black and white vehicles have similar price distributions. Red vehicles show slightly lower prices, possibly due to lower demand or different vehicle types.

## Models performance
Regarding the performance of the Lasso and Ridge models used in the previous section, it is worth mentioning the high difference between their final scores both at training and testing, where Ridge shows much better behaviour at detecting the attributes which contribute more to the price variable.

**Lasso scores**

Training R²: 53.06% Testing R²: 50.80%

**Ridge scores**

Training R²: 66.38% Testing R²: 57.90%

To improve the performance of both models we could change the hyperparameters to have more cross-validation foldings, scaling or normalization of numerical values.
Based on the previous list we can clearly see that the **most important features to take into account in the price of the cars are the region, the manufacturer, model, drive and type**
