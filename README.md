# model_evs

# Effective Incentives for Electrical Vehicles (EVs) in the US

# Summary
Adoption of electric vehicles (EVs) is a key part of reducing greenhouse gas emissions. Using EV sales numbers in each US state, I built a regression model to predict sales, and investigated the impact of incentive policies and other factors on EV adoption.

# Problem Statement
Reducing carbon dioxide (CO2) emissions is one of the greatest challenges of our time. In 2021, carbon emissions from transportation accounted for 28% of total U.S. greenhouse gas emissions, making it the sector with the largest contribution. Federal and state governments have already spent over $20 billion dollars to incentivize people to buy low emission vehicles such as hybrid and electric vehicles. However, less than 5% of the cars on the road today are zero emission vehicles, indicating that a lot more investment is needed. Identifying the best way for a state government to use their limited incentive budget to maximize the adoption of low emission vehicles is an important question for policy makers as well as for other stakeholders such as electricity generation companies. Currently state-level incentives for buying EVs vary widely from thousands of dollars in tax credits for some states all the way to an annual penalty of $200 dollars per year in others. Using EV sales numbers in each US state and machine learning, I built a regression model to predict sales, and investigated the impact of incentive policies and other factors on EV adoption. I added other factors into the model to improve its predictive accuracy, including annual state-level registration fees, available number of charging stations in each state, and political orientation. Policy makers, electricity generation companies and other stakeholders can use these findings when determining the best policies around EV incentives and electricity consumption going forward.

# Project
I used vehicle registration data from the U.S. Department of Energy's Alternative Fuels Data Center (https://afdc.energy.gov/vehicle-registration) to estimate EV sales number in each state for each year from 2016 to 2022. I then built and compared several regression models (ridge, decision tree, random forest) to predict EV sales, and investigated the impact of state incentive policies and other factors (by state and by year) on EV adoption. The data were obtained from several public sources, referenced below. Features included in the regression models are shown below together with the corresponding data sources: 
(1) state-level incentives from Tax Foundation (https://taxfoundation.org/data/all/state/electric-vehicles-ev-taxes-state/) and Wikipedia (https://en.wikipedia.org/w/index.php?title=Plug-in_electric_vehicles_in_the_United_States#Government_support, and revision history of this page)
(2) annual registration fees from Tax Foundation (https://taxfoundation.org/data/all/state/electric-vehicles-ev-taxes-state/)
(3) available number of charging stations in each state from the U.S. Department of Energy's Alternative Fuels Data Center (https://afdc.energy.gov/files/docs/historical-station-counts.xlsx?year=2023)
 (4) political leaning of each state from The Cook Political Report (https://www.cookpolitical.com/2020-national-popular-vote-tracker).

In this notebook, I employed the following procedure for predictive modeling of EV sales:
1. Scraped, cleaned, and merged data from multiple sources (see references above)
2. Plotted the data
3. Created and trained regression models
4. Evaluated performance (cross validation, test)
5. Interpreted results and discussed future directions



Data sources:
1. Vehicle Registration Counts by State and Fuel Type https://afdc.energy.gov/vehicle-registration
2. How Are Electric Vehicles Taxed in Your State? https://taxfoundation.org/data/all/state/electric-vehicles-ev-taxes-state



