# Homework 1 - ME597

Jeff Seufer

## Problem 1

### Scoring and Weighting Methods

When using scoring and weighting, the user will create a list of tests to evaluate the performance of different design alternatives.  Scoring is assigned based on rank order of how favorable a test result is when compared to its peers.  The least favorable solution receives zero points, then next least receives one point, up until the most favorable solution receives the most points (n-1 points, where n is the number of alternatives being considered).  Weighting may be introduced as a multiplier in case specific criteria are more critical to the success of the end product.  Examples such as safety, cost, and time to develop may be given high weights so that impractical decisions are easily discarded.

Examples can be at a low level, such as performing material selection by analyzing various material properties, or at a higher level such as selecting a large system by assigning factors of the subsystems that are important to the end user.  Scoring and weighting has the advantage of head to head comparison of final solutions, but it will not provide insight into parameters that are much better than others.  This will provide a gap in identifying true differentiators in the market.  For example, if item A is $1, item B is $200, and item C is $250, the resultant scores of 2 points for item A, 1 point for item B, and 0 points for item C will not tell the full story of the different options, even with a high weight multiplier assigned.   This process is also prone to irrelevant alternatives.  This phenomena occurs when a poor solution ranks highly in a couple of tests.  These high rankings will artificially cause otherwise high performing options to appear poor.  If an option is clearly not the best solution, it should be removed from this type of study as it may skew the overall comparison.  

### Analytical Hierarchy Process (AHP)

This process is similar to Scoring and Weighting, but it will assign a linearized value to each scoring criteria.  Traditionally, the most undesirable result from the group of options will receive zero points, while the most desirable will receive one point.  Points that are not at the minimum or maximum will be given a score based on the linear normalization between the end points.  The scores are tallied across all criteria and designs can be ranked based on these outputs.  

The linearization of scores will introduce more granularity to the decisions being made.  In the case of 3 alternatives, a parallel can be drawn to Scoring and Weighting that the most favorable solution receives one point, the next best receives a half point, and the least favorable receives zero points.  With the linearized values of AHP, the middle solution may receive scores that are closer to the extremes.  This allows for more or less differentiation when the spread of the criteria is high.

This addresses some of the gap of relevant importance from Scoring and Weighting, but it still is prone to irrelevant alternatives.  If there are certain factors (cost, safety) that are very important, additional weights will need to be applied to these factors in order to keep infeasible solutions from appearing as the preferred selection.  When adding weights to adjust for these method disadvantages, it is very important that the decision maker does not introduce additional bias towards which designs are preferred.

### Similarities and Differences

These methods are very similar to each other and should be used with caution when making important decisions.  Scoring and Weighting will perform best with few design alternatives and a limited set of tests or appropriate weightings assigned.  AHP will address some gaps in Scoring and Weighting by adding the feature of linearized performance for each attribute.  Both processes require careful consideration from the decision maker to be sure that poor designs are not influencing the performance of other higher performing designs. In the worst case, both methods are prone to choosing infeasible designs if the detailed scores and criteria are not reviewed carefully.

\newpage

## Problem 2 - Application

Three new vehicles will be compared for purchase.  A table below will summarize the key features of these vehicles and the data will be applied to the two decision making techniques listed above.

### Alternatives - Raw Data

Vehicle types:

A. 2021 Honda Civic

B. 2021 Toyota Corolla

C. 2021 Mazda 3

### Dimensions

| Vehicle | Vehicle weight [lbs] | Vehicle Length [in] | Front Headroom [in] | Rear Legroom [in] | Luggage Space [cu ft] |
| :-----: | :------------------: | :-----------------: | :-----------------: | :---------------: | :-------------------: |
|    A    |         2955         |        177.9        |        37.6         |        36         |         25.7          |
|    B    |         3150         |        182.5        |         38          |       34.8        |         13.1          |
|    C    |         3268         |        183.5        |        37.6         |       35.1        |         13.2          |

### Powertrain

| Vehicle | Engine displacement [liters] | Turbo or n/a | Power [hp] | Trans-mission | Torque [ft-lbs] | Driven Wheels |
| :-----: | :--------------------------: | :----------: | :--------: | :-----------: | :-------------: | :-----------: |
|    A    |             1.5              |    Turbo     |    174     |      CVT      |       162       |       2       |
|    B    |             2.0              |     n/a      |    169     |      CVT      |       151       |       2       |
|    C    |             2.5              |     n/a      |    186     |   6 sp auto   |       186       |       4       |

### Performance

| Vehicle | 0-60 Time [s] | 70-0 Distance [ft] | Skidpad [g] | Highway Fuel Economy [mpg] | City Fuel Economy [mpg] |
| :-----: | :-----------: | :----------------: | :---------: | :------------------------: | :---------------------: |
|    A    |      7.2      |        170         |     .91     |             40             |           31            |
|    B    |      8.0      |        174         |     .82     |             36             |           29            |
|    C    |      8.1      |        169         |     .85     |             33             |           25            |

### Features

| Vehicle | Sunroof | Wheel Size [in] | Audio Speakers | Infotainment Screen size [in] | Heated Seats |
| :-----: | :-----: | :-------------: | :------------: | :---------------------------: | :----------: |
|    A    |   Yes   |       17        |       8        |               7               |     Yes      |
|    B    |   Yes   |       18        |       6        |               8               |     Yes      |
|    C    |   No    |       18        |       8        |              8.8              |     Yes      |

\newpage

### Pricing

|          Vehicle Package          | Standard Cost |                            Source                            |
| :-------------------------------: | :-----------: | :----------------------------------------------------------: |
| 2021 Honda Civic EX CVT Hatchback |    $24,700    | [Honda Official Website](https://automobiles.honda.com/civic-hatchback/specs-features-trim-comparison),<br/> [Car and Driver](https://www.caranddriver.com/honda/civic-2021) |
|      2021 Toyota Corolla XSE      |    $25,925    | [Toyota Official Website](https://www.toyota.com/corolla/2021/features/multimedia/1882/1866/1860),<br/>[Car and Driver](https://www.caranddriver.com/toyota/corolla) |
|     2021 Mazda3 Preferred AWD     |    $25,750    | [Mazda Official Website](https://www.mazdausa.com/vehicles/2021-mazda3-sedan/compare-vehicle-specs-and-trims),<br/>[Car and Driver](https://www.caranddriver.com/mazda/mazda-3) |

\newpage

## Decisions

### Scoring and Weighting Matrix

| Tests - Dimension                  | Best | Middle | Worst |
| ---------------------------------- | ---- | ------ | ----- |
| Vehicle Weight (lowest preferred)  | A    | B      | C     |
| Vehicle Length (lowest preferred)  | A    | B      | C     |
| Front Headroom (highest preferred) | B    |        | A,C   |
| Rear Legroom (highest preferred)   | A    | C      | B     |

| Tests - Powertrain                      | Best | Middle | Worst |
| --------------------------------------- | ---- | ------ | ----- |
| Engine Displacement (highest preferred) | C    | B      | A     |
| Turbo (preferred)                       | A    |        | B,C   |
| Power (highest preferred)               | C    | A      | B     |
| Transmission (CVT preferred)            | A,B  |        | C     |
| Torque (highest preferred)              | C    | A      | B     |
| Driven wheels (4 preferred)             | C    |        | A,B   |

| Tests - Performance                      | Best | Middle | Worst |
| ---------------------------------------- | ---- | ------ | ----- |
| 0-60 Time (lowest preferred)             | A    | B      | C     |
| 70-0 Distance (lowest preferred)         | C    | A      | B     |
| Skidpad (highest preferred)              | A    | C      | B     |
| Highway Fuel economy (highest preferred) | A    | B      | C     |
| City Fuel economy (highest preferred)    | A    | B      | C     |

| Tests - Features and Cost       | Best  | Middle | Worst |
| ------------------------------- | ----- | ------ | ----- |
| Sunroof (preferred)             | A,B   |        | C     |
| Wheel size (highest preferred)  | B,C   |        | A     |
| Speaker (highest preferred)     | A,C   |        | B     |
| Screen size (highest preferred) | C     | B      | A     |
| Heated Seats (preferred)        | A,B,C |        |       |
| Price (lowest preferred)        | A     | C      | B     |

\newpage

The Scoring and Weighting results are summarized in the following tables.  Two approaches are taken to show how the survey can produce different results based on summary methods.  It is important to note that all tests are given equal weight for the sumarry of the first table.  This will ensure that no biasees are introduced by myself as the decision maker and it can be conceived that I am searching for the best all-around vehicle.  The first table simply includes the sum of points from the Scoring table above.  In the second table, the Dimension, Powertrain, Performance, and Features sections are all given equal weights as a sub-category.  In this case, car model A is still the winner, but the margin but which it performs is drastically higher.

| Method 1 - All Tests | Car A | Car B | Car C |
| -------------------- | ----- | ----- | ----- |
| Score:               | 29    | 16    | 20    |

| Method 2 - Subcategory | Car A | Car B | Car C |
| ---------------------- | ----- | ----- | ----- |
| Dimension Score        | 2     | 1     | 0     |
| Powertrain Score       | 1     | 0     | 2     |
| Performance Score      | 2     | 0     | 0     |
| Features Score         | 2     | 0     | 0     |
| Total Score            | 7     | 1     | 2     |

\newpage

### AHP

| Tests - Dimension                  | A    | B    | C    |
| ---------------------------------- | ---- | ---- | ---- |
| Vehicle Weight (lowest preferred)  | 1    | .377 | 0    |
| Vehicle Length (lowest preferred)  | 1    | .179 | 0    |
| Front Headroom (highest preferred) | 0    | 1    | 0    |
| Rear Legroom (highest preferred)   | 1    | 0    | .25  |

| Tests - Powertrain                      | A    | B    | C    |
| --------------------------------------- | ---- | ---- | ---- |
| Engine Displacement (highest preferred) | 0    | .5   | 1    |
| Turbo (preferred)                       | 1    | 0    | 0    |
| Power (highest preferred)               | .294 | 0    | 1    |
| Transmission (CVT preferred)            | 1    | 1    | 0    |
| Torque (highest preferred)              | .458 | 0    | 1    |
| Driven wheels (4 preferred)             | 0    | 0    | 1    |

| Tests - Performance                      | A    | B    | C    |
| ---------------------------------------- | ---- | ---- | ---- |
| 0-60 Time (lowest preferred)             | 1    | .111 | 0    |
| 70-0 Distance (lowest preferred)         | .8   | 0    | 1    |
| Skidpad (highest preferred)              | 1    | 0    | .333 |
| Highway Fuel economy (highest preferred) | 1    | .429 | 0    |
| City Fuel economy (highest preferred)    | 1    | .377 | 0    |

| Tests - Features and Cost         | A    | B    | C    |
| --------------------------------- | ---- | ---- | ---- |
| Sunroof (preferred)               | 1    | 1    | 0    |
| Wheel size (highest preferred)    | 0    | 1    | 1    |
| Speaker Count (highest preferred) | 1    | 0    | 1    |
| Screen size (highest preferred)   | 0    | .556 | 1    |
| Heated Seats (preferred)          | 1    | 1    | 1    |
| Price (lowest preferred)          | 1    | 0    | .143 |

| Results - All totals | Car A  | Car B | Car C |
| -------------------- | ------ | ----- | ----- |
| Sum:                 | 13.552 | 7.529 | 9.583 |

### Selection

In all cases, Car A is the "best" car.  Based on the criteria selected, the decision maker should choose the Honda Civic for their next vehicle.  Some biases do exist in this case, but not necessarily within the methods.  In this case, many of the design tests are dependent on each other.  If a car has a lot of power or it is light, it will greatly affect the 0-60 time of the vehicle.  If a car has a large engine, it may produce more power than a car with a turbocharger, even though the scores indicate that a turbo is preferred.  This is an example of how important it is to select independent and important design criteria.  Additionally, this will highlight the importance of choosing criteria that are performance based and not feature based.  As an end customer, we are searching for a car that meets certain performance requirements (fast, sporty, practical) and must keep in mind that the method by which these criteria are met can be held separate from the end function.

One more factor influencing this study is the lack of weights assigned to the tests.  In some cases, factors that meet and exceed a certain threshold should be given the same weighting.  It may be true that there is no extra utility to the decision maker as long as there is at least 37 inches of headroom in the front of the car.  As long as that individual fits comfortably, there may be little value in additional space.  Similarly, we can apply extra weighting to features such as four wheel drive.  If the customer lives in a location with harsh winters, it would be common that Car C with all wheel drive will provide a valuable trade off for weight and quickness in exchange for safety on hazardous snowy roads.

\newpage

## Problem 3 - Evaluation

### Part a

There are some decisions made in this study that introduce preferences of the decision maker.  In one case, engine size, it is noted that a larger engine is preferred.  This assumption is created in a way that the decision maker likely prefers the power that is generally associated with a large engine.  To contrast this, some users may actually prefer a smaller engine based on the general theory that these will produce better fuel economy for the vehicle.  Other preferences may arise in the headroom and legroom tests.  If the decision maker is small in stature, headroom may not be a consideration that has any importance.  Similarly, if the decision maker has no children or does not plan to drive multiple people in their car frequently, the rear legroom may be irrelevant to the user.  These issues can arise within both methods equally.  Biases will always be present in some capacity, and it is important that all customers are involved during weighting and priority discussions.  As the sole purchaser and decision maker, preferences appearing in the matrices may be acceptable.

### Part b

Both decision making methods are able to utilize all of the available information.  As discussed in earlier sections, the inability of the Scoring and Weighting method to differentiate factors that are much better or much worse indicates that it is prone to not using the information to the extent that could be necessary to provide an accurate summary.  Some information that was needed but not available would be the priority or weights of each factor from the decision maker.  We know that the goal was to select a compact car, but we do not know the intended use of that car.  If the decision maker was looking for their next vehicle to take to the racetrack on the weekend, it will imply very different requirements than someone looking for their next family vehicle or child's first car.

### Part c

The Favorable Properties of a Selection Method highlight ten goals for all decision making methods.  Both methods are succesful when it comes to providing a rank order of design alternatives, allowing the comparison under conditions of uncertainty, being independent of engineering discipline, staying consistent regardless of order of consideration, not imposing constraints on the decision, and welcoming additional information.  Both AHP and Scoring and Weighting are prone to imposing preferences as weighting the tests is welcome and encouraged through these methods.  These methods are also vulnerable to irrelevant alternative bias, which means that they do not fulfill the tenets of making decisions against all subsets of the options and robustness to new designs causing high performers to appear less favorable.  The final point, being self-consistent and logical, provides a slight edge to AHP.  Because of the linearization of results, this method is able to provide deeper insight and maximize the use of available information.

### Part d

Overall, these two processes are very similar and will often yield similar results.  When making decisions as a team, both methods can be utilized with caution to produce great success.  When cross-functional teams are assigned with filling out these matrices, biases from individuals will be greatly reduced.  Each member will have different priority based on design, cost, timelines, manufacturability, etc. and these will show up in the final product.  Both methods will also require that the categories upon which decisions are made are appropriate for all parties.  Sub-categories can help address these issues.  For example, if there are 25 criteria from the design team and only 10 criteria from the manufacturing team, it is important that the results of each sub-category are comparably weighted and the team with less criteria is not dominated in the final solution.  As in all decisions, it is important that the requirements for the end product are clearly defined so that relevant information can be the focus throughout the decision making process.