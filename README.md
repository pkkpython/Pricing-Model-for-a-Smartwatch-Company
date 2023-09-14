# Pricing Model for a Smartwatch Company

![](Order%20Quantity%20Modelling%20Model%202.png)

## Overview

Welcome to the Pricing Model for a Smartwatch Company project! This project aims to help NuWave, a smartwatch manufacturer, make informed pricing decisions for their new flagship product. As a business analyst at Analytics, your task is to create a comprehensive pricing model that considers various factors such as market share, profit margins, storage costs, and market demand.

This GitHub repository contains all the resources and code needed to tackle the project's challenges. We'll break down the project into milestones, each addressing a specific aspect of the pricing model.

## Understand the Problem

NuWave is a startup dealing in a wide range of electronic gadgets and accessories. They manufacture their own products but procure raw materials from other companies since they can't afford to build their own research and development department at present.
Situation

NuWave wants to launch a new smartwatch, which will be one of their flagship products. They plan to launch the watch with an OLED display.
They intend to first enter the market and gain at least 5% of the market share.
As a new player in the smartwatch market, they want to price the watch lower than their competition (selling at ₹ 7,799).
To achieve 5% of the market share, NuWave needs to sell at least 1,800 units per day. Assume NuWave can completely fulfill the demand for the day.

## Complication

For NuWave to sell 1,800 smartwatches a day, they need to have a certain level of inventory.
Each smartwatch requires one OLED panel. For smooth production, they need to have its stock as well.
NuWave can store only 2000 OLED panels in their own facility. To store more, they need a warehouse, which will cost them ₹ 12,000/day. They can store 10,000 OLED panel units in one warehouse.
The warehouse should not be underutilized.
Now, as a business analyst at NuWave, your job is to find out:
At what price should they sell one unit, to gain a 5% market share and earn at least a 2% profit margin?
Minimum order quantity of panels at that price point so NuWave doesn't make a loss.

## Key Expectations
**Build a spreadsheet model to find out the selling price of one smartwatch so that:**
- NuWave can gain a 5% market share.
- Earn at least a 2% profit margin.


## First Submission

Hey there! Before we start with the actual problem, try solving a mini version of the problem here. It will boost your confidence and clear some concept.
**Case**
NuWave wants to test their smartwatch before launching. They intend to sell 500 units for testing.
They approached Samsung to acquire OLED panels for their watch. Samsung quoted the price as given below.

| Quantity | Per Unit Cost |
|---------|--------------|
| 1       | ₹ 1,750      |
| 1000    | ₹ 1,575      |


Based on your understanding in this objective, answer the below question and validate your work.

Here we have to use linear relationship to find the per unit cost of a smartwatch incurred by NuWave.

A linear relationship is a fundamental concept in mathematics and statistics that describes a straight-line relationship between two variables. In a linear relationship, as one variable changes, the other variable changes proportionally in a consistent manner. This relationship is often represented by a linear equation or a straight-line graph.

Equation Form: 
The general form of a linear equation is:
y = mx + b
 "y" is the dependent variable.
"x" is the independent variable.
"m" is the slope of the line, representing the rate at which "y" changes with respect to changes in "x."
"b" is the y-intercept, which is the value of "y" when "x" is zero. It's the point where the line crosses the y-axis.

Slope: The slope of the line indicates the rate of change between the variables. It represents how much "y" changes for a unit change in "x." A positive slope means that as "x" increases, "y" also increases, while a negative slope means that as "x" increases, "y" decreases.

Y-Intercept: The y-intercept is the point where the line crosses the y-axis. It gives the value of "y" when "x" is zero. In other words, it's the initial value of the dependent variable "y" before any changes in the independent variable "x."

Here the price of panels depends linearly on the number of units ordered. The higher the quantity order, the lower the per-unit cost.  
Here y is the per unit cost and x is the order quantity. When the order quantity increases the per unit cost decreases, or the value of slope(m) would be negative.
Negative Slope (m < 0): When the value of "m" is negative, it indicates that as the independent variable "x" increases, the dependent variable "y" decreases. This is a negative correlation between the variables. For instance, as the temperature (x) increases, the demand for winter clothing (y) might decrease.

In this context, a linear relationship refers to the correlation between two variables (in this case, quantity and cost) that can be described by a straight-line equation. When you plot the data points on a graph, they form a straight line, hence the term "linear."

In summary, the linear relationship is established using the slope formula to determine the cost decrease rate with increasing quantity. Then, the point-slope formula helps calculate the specific cost for a given quantity. Finally, the total cost is computed by adding the cost of OLED panels and the fixed component cost.

Let's break down the steps used to establish and utilize the linear relationship between the quantity of OLED panels ordered and the per unit cost:

Step 1: Data Points
The given information provides two data points:

Quantity: 1, Per Unit Cost: ₹1,750
Quantity: 1000, Per Unit Cost: ₹1,575
These points represent the quantity of panels ordered and their respective per-unit costs.

Step 2: Calculate the Slope
The slope of the line (m) represents the rate of change of the cost with respect to the quantity. It can be calculated using the formula:

Slope (m) = (Change in Y) / (Change in X) = (Cost at Quantity 2 - Cost at Quantity 1) / (Quantity 2 - Quantity 1)

Substituting the values:
Slope (m) = (₹1,575 - ₹1,750) / (1000 - 1)
= ₹-175 / 999
≈ -₹0.175

The negative slope indicates that as the quantity increases, the cost decreases.

Step 3: Using the Point-Slope Formula
The point-slope formula of a linear equation is:

y - y1 = m(x - x1)

Here, y represents the cost, x represents the quantity, (x1, y1) is one of the given data points.

Using the first data point (1, ₹1,750):

Cost - ₹1,750 = -₹0.175 * (Quantity - 1)

Step 4: Calculate the Cost
Now, substitute the quantity of 500 units into the equation:

Cost - ₹1,750 = -₹0.175 * (500 - 1)
Cost - ₹1,750 = -₹0.175 * 499
Cost = ₹1,750 - ₹87.325
Cost ≈ ₹1,662.675

Step 5: Total Cost
Since the cost of other components of the smartwatch remains fixed at ₹6,000, you simply add this fixed cost to the calculated cost of the OLED panels:

Total Cost = Cost of OLED panels + Cost of other components
Total Cost = ₹1,662.675 + ₹6,000
Total Cost ≈ ₹7,662.675

Rounding to two decimal places, you get ₹7662.59, which is the closest option to the calculated value.

To calculate the price NuWave should set for one smartwatch in order to earn a profit margin of at least 1%, we need to consider the cost of production and the desired profit margin.

From the previous calculations, we know that the cost of producing one smartwatch (including OLED panels and other components) is approximately ₹7,662.59.

To calculate the selling price with a profit margin of 1%, we need to add 1% of the cost to the cost itself:

Profit Margin = 1% = 0.01
Desired Selling Price = Cost + (Cost * Profit Margin)
Desired Selling Price = ₹7,662.59 + (₹7,662.59 * 0.01)
Desired Selling Price = ₹7,662.59 + ₹76.6259
Desired Selling Price ≈ ₹7740.2159

Rounded to two decimal places, the closest option is ₹7740. Therefore, the correct answer is: ₹7740


### Steps:

- Finding Cost per Unit

- Calculating Total Cost

- Calculating Selling Price


## Project Deliverables

Upon completing all milestones, you should be able to:

- Determine the selling price that allows NuWave to achieve a 5% market share and maintain a minimum 2% profit margin.
- Calculate the minimum order quantity of OLED panels at that price point to avoid losses.
- Provide recommendations and insights based on the analysis.

## Conclusion

This project will empower NuWave to make data-driven decisions when pricing their smartwatches, ensuring competitiveness in the market while maintaining profitability. Feel free to explore each milestone and contribute to the development of the pricing model.






