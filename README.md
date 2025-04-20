The aim of this Python code is to analyze and compare the economic cost and environmental impact of different power generation portfolios over a 10-year planning period, and to perform a Cost-Benefit Analysis (CBA) of investing in a 100 MW solar power project.
This is done by: 
Forecasting electricity demand over 10 years.
Evaluating the Net Present Value (NPV) of system costs for different mixes of power generation technologies (coal, solar, wind).
Calculating the benefits (cost savings and emission reductions) of deploying solar power to replace coal generation.
1. Forecast Electricity Demand
The code estimates electricity demand over the next 10 years.

It starts with a base demand of 1000 MW in the first year and assumes a 4% annual growth rate.

2. Define Power Generation Resources
Four resources are considered: coal, solar, wind, and battery.

Each resource is defined by:

CapEx (Capital Cost): Cost to build capacity (₹/MW)

O&M Cost: Annual operation and maintenance (₹/MW)

Fuel Cost: Fuel expense per unit of energy (₹/MWh)

Emissions: CO₂ emissions per MWh

Capacity Factor (CF): Average usage of capacity across the year

3. Define Portfolios (Generation Mixes)
Three different portfolios are considered:

All coal

50% solar + 50% coal

30% wind + 30% solar + 40% coal

These portfolios specify what percentage of the annual demand is met by each technology.

4. Calculate System Cost for Each Portfolio
For each year:

The code calculates how much capacity of each resource is needed to meet the forecasted demand.

It estimates the annual cost, including:

Annualized CapEx (spread over 10 years)

O&M cost

Fuel cost

Emission cost (using a carbon price of ₹1000 per ton)

The total yearly cost is then converted into a Net Present Value (NPV) to account for the time value of money.

5. Display Portfolio Costs
The code prints the total NPV of system cost for each portfolio over 10 years, helping compare the economic impact of each generation mix.

6. Cost-Benefit Analysis (CBA) for 100 MW Solar Project
The code evaluates if installing 100 MW of solar power is economically beneficial.

It calculates:

Energy generated annually by the solar plant

Cost savings from avoided coal fuel use and carbon emissions

Investment cost (CapEx in year 1 and O&M annually)

NPV of benefits and costs over 10 years

Net NPV (benefit - cost)
