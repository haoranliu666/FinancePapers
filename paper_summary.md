# FinancePapers

### Political Uncertainty and Corporate Investment Cycles

During election years, firms reduce investment expenditures by an average of 4.8% relative to nonelection years.

Univariate analysis: Corporate investment over total asset at -2, -1, 0, +1, +2 years

Multivariate analysis: Investment = ElectionDummy + Q + CF + GDPgrowth + FirmFE + TimeFE + control

Tobin Q is a proxy for the incentive to invest.

Variation analysis: I = Elect\*X + Elect + X + control

X can be:

1. common law countries vs. civil law countries
2. presidential system vs. parliamentary system
3. checks and balances measure
4. government stability measure
5. ratio of central government spending to GDP

### Did securitization lead to lax screening? Evidence from subprime loans

Regressional Discontinuity Design. 

Using FICO score, 620.

### Big Bad Banks? The Winners and Losers from Bank Deregulation in the United States

Studied causal impact of bank regulations on income distribution using a two-way fixed effect difference-in-difference design.

Random treatment validation:

Neither the level nor rate of change in the distribution of income before deregulation help predict when a state removed restrictions on bank branching, suggesting that the timing of branch deregulation at the state level is exogenous to the state’s distribution of income.

```diff
- DID

- Difference-in-differences setting:

Dependent variables are measurements of income inequality. 

(1) Gini coefficient; 

(2) Theil index; 

(3) difference between the natural logarithm of incomes of those at the 90th percentile and those at the 10th percentile; 

(4) difference between the natural logarithm of incomes of those at the 75th percentile and those at the 25th percentile.

Core intersection item is Treat X Post.

Control for growth rate of per capita Gross State Product (GSP), unemployment rate, and other state-level time varying attributes, year-state fixed effects, allowing for state-level clustering of the errors.
```

### Sex, Drugs, and Bitcoin: How Much Illegal Activity Is Financed through Cryptocurrencies?

An RFS paper about bitcoin and illegal activity

about half of bitcoin transations involve in illegal activity

network algorithm; bitcoin blockchain;   users -> illegal users

illegal users transact more, with smaller transactions,  denser network

intrinsic value of bitcoin

1. seized users
2. darknet wallet
3. darknet forum


### Option Momentum

Stock options with high historical returns continue to outperform options with low returns.

### The Real Effects of Environmental Activist Investing*

Environmental activist investing targeted firms reduce their toxic releases, greenhouse gas emissions, and cancer-causing pollution. Using DID-PSM on Boardroom Accountability Project (BAP) event. Compares outcomes for plants of firms targeted by the BAP to plants of similar firms that were not targeted by the BAP.

Data: Compustat, CRSP, Institutional Shareholder Services (ISS), and Thomson Reuters ASSET4 database, plus BAP and other enviromental related data.


```diff
- PSM + DID

- Matching covariates: 
Firm size, return on assets, market-to-book ratio, and ASSET4 score

- Difference-in-differences setting:

Dependent variables can be logarithm of emissions without or with scaling. 

Core intersection item is Environment X Post.
Environment 
= 1 if if the BAP targets the firm for environmental reasons. 
Post 
= 1 for the firm-year following the first target year of the BAP.

Control for plant-chemical fixed effects, and chemical-year fixed effects.
```

### Mortgage Markets with Climate-Change Risk: Evidence from Wildfires in California

Causal relationship between mortgage performance (i.e., delinquency and foreclosure) and climate-change-driven events (i.e., wildfires), using 4 databases: 1. Wildfire events; 2. Mortgage characteristics and performance; 3. Mortgage geolocation and property characteristics; 4. Weather.


```diff
- DID + Panel

- 1 Difference-in-differences setting:

Dependent variables can be delinquency or foreclosure of a morgage. 

Core intersection item is Treatment X Afterfire.
Treatment 
= 1 if active mortgage falls inside the wildfire zone and 0 otherwise; 
Afterfire 
= 1 if after the fire and 0 otherwise;

Control for mortgage characteristics.

- 2 Difference-in-differences setting:

Dependent variables and controls are same as above. 

Core intersection item is Treatment X Afterfire X Bigfire(1or2).
Bigfire1 
= the number of mortgages affected by the wildfire;
Bigfire2
= 1 if the mortgage is affected by a fire that is 1 sd above the average
wild fire in terms of mortgages affected.

- 3 Panel + IV setting:
IV: maximum temperature of the month in the location of the property.
```

Part of the DID result

<img src="https://github.com/haoranliu666/FinancePapers/blob/main/images/Mortgage%20Markets%20with%20Climate-Change%20Risk.png" width="50%" height="50%">

IV result:

<img src="https://github.com/haoranliu666/FinancePapers/blob/main/images/Mortgage%20Markets%20with%20Climate-Change%20Risk_IV.png" width="50%" height="50%">





LTV denote the dynamic loan-to-value for each mortgage at each month

### Are Judges Like Umpires? Political Affiliation and Corporate Prosecutions

Judges appointed by a democrat president impose larger fines for corporate crimes involving environmental and labor regulations while Republican-appointed judges impose larger fines for crimes involving the hiring of illegal immigrants.

To assess whether judicial political affiliations affect the outcomes of corporate prosecutions, they construct data on federal corporate prosecutions and the political affiliation of federal judges, which are nominated by the President for lifetime appointments. And judges do have political preferences. Once cases are assigned to a prosecution office in the US, 
a judge is **randomly selected** from the federal judges that preside over that particular jurisdiction.

```diff
- Difference-in-differences setting:

Dependent variables can be the type of decision of guilt, or fine. 

Core intersection item is Democrat X DemocratTilt
Democrat 
= 1 if the judge is nominated by a Democrat President, 
= 0 if Republican.
DemocratTilt 
= 1 if cases involving labor or environmental crimes;
= -1 if immigration crimes; 
= 0 if crimes that do not easily lend themselves to a partisan classification.

Control for judge, crime type, and year fixed effects.
```

### Do Shareholders Gain from Their Right to Sue? Evidence from Federal Judge Turnover

Shareholders’ right to sue corporations and managers for breach of securities laws causes equity value loss.

While federal securities laws are the same across all public firms and U.S. states, federal judges likely exercise considerable discretion in the actual enforcement of these laws and hence influence the outcomes of shareholder lawsuits. They classify U.S. federal judges’ as pro-shareholder or pro-business and show that pro-shareholder judges are indeed more likely to rule against (in favor of) the early dismissal of shareholder lawsuit. Use judicial turnover events in federal court as shocks to shareholders’ right to sue, and study the impact of stronger shareholder rights for equity value. Examine abnormal stock returns around judicial turnover events that affect the average friendliness of a court toward shareholder rights.

```diff
- Fixed effect setting:

Dependent variable is cumulative abnormal stock return of the firm in the 41 days around the change in court composition.

Key regressor Change in ProShareholder 
= 1  if a judicial turnover increases the shareholder-friendliness of district court k where the firm headquartered;
= -1 if the judicial nomination decreases the shareholder-friendliness of that court;
= 0 for firms in the comparison group, i.e., unexposed firms.

Control for some company characteristics, district fixed effects, state × date fixed effects.
```

### Grit and Credit Risk: Evidence from Student Loans

Students who quit courses during college are 13% more likely to default on student loans than their perseverant peers, controlling for conventional risk factors. Students who voluntarily repeat courses after performing poorly are 13% less likely to default than peers who give up.

Data unavailable, fixed effect.

### Peer Effect in Product Adoption*

A new phone purchase by a friend has a large positive and long-term effect on an individual’s own demand for phones of the same brand, most of which is concentrated on the particular model purchased by the friend. 

Their most basic specification seeks to understand a Facebook user’s decision to buy a new phone in a given week as a function of the prior or contemporaneous purchases of her friends. But observing a correlation in purchasing behavior within friendship groups does not necessarily provide evidence for peer effects, like an Apple enthusiast may primarily be friends with other Apple enthusiasts. So they develop **two instrumental variables** for the purchasing behavior of a person’s friends: the number of a user’s friends who randomly lose their phones, and the number of friends who have owned their phones for exactly two years, using NLP on Facebook de-identified data.

IV-2SLS.

