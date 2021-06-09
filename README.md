# FinancePapers
Summary of some finance papers I'm interested in.

## AFA2021

### Paper: Are Judges Like Umpires? Political Affiliation and Corporate Prosecutions

Judges appointed by a democrat president impose larger fines for corporate crimes involving environmental and labor regulations while Republican-appointed judges impose larger fines for crimes involving the hiring of illegal immigrants.

To assess whether judicial political affiliations affect the outcomes of corporate prosecutions, they construct data on federal corporate prosecutions and the political affiliation of federal judges, which are nominated by the President for lifetime appointments. And judges do have political preferences. Once cases are assigned to a prosecution office in the US, a judge is **randomly selected** from the federal judges that preside over that particular jurisdiction.

##### Difference-in-differences setting:

Dependent variables can be the type of decision of guilt, or fine if pleaded guilty. 

Core intersection item is Democrat X DemocratTilt

Democrat = 1 if the judge is nominated by a Democrat President, 0 if Republican.

DemocratTilt = 1 if cases involving labor or environmental crimes; -1 if immigration crimes; 0 if crimes that do not easily lend themselves to a partisan classification, like fraud, money laundering, and bribery 

Control for judge, crime type, and year fixed effects.

### Paper: Do Shareholders Gain from Their Right to Sue? Evidence from Federal Judge Turnover

Shareholders’ right to sue corporations and managers for breach of securities laws causes equity value loss.

While federal securities laws are the same across all public firms and U.S. states, federal judges likely exercise considerable discretion in the actual enforcement of these laws and hence influence the outcomes of shareholder lawsuits. They classify U.S. federal judges’ as pro-shareholder or pro-business and show that pro-shareholder judges are indeed more likely to rule against (in favor of) the early dismissal of shareholder lawsuit. Use judicial turnover events in federal court as shocks to shareholders’ right to sue, and study the impact of stronger shareholder rights for equity value. Examine abnormal stock returns around judicial turnover events that affect the average friendliness of a court toward shareholder rights.

##### Fixed effect setting:

Dependent variable is cumulative abnormal stock return of the firm in the 41 days around the change in court composition.

Key regressor Change in ProShareholder = 1  if a judicial turnover increases the shareholder-friendliness of district court k where the firm headquartered, or it is equal to -1 if the judicial nomination decreases the shareholder-friendliness of that court, equal to 0 for firms in the comparison group, i.e., unexposed firms.

Control for some company characteristics, district fixed effects, state × date fixed effects.

### Paper: Grit and Credit Risk: Evidence from Student Loans

Students who quit courses during college are 13% more likely to default on student loans than their perseverant peers, controlling for conventional risk factors. Students who voluntarily repeat courses after performing poorly are 13% less likely to default than peers who give up.

Data unavailable, fixed effect.

### Paper: Peer Effect in Product Adoption*

A new phone purchase by a friend has a large positive and long-term effect on an individual’s own demand for phones of the same brand, most of which is concentrated on the particular model purchased by the friend. 

Their most basic specification seeks to understand a Facebook user’s decision to buy a new phone in a given week as a function of the prior or contemporaneous purchases of her friends. But observing a correlation in purchasing behavior within friendship groups does not necessarily provide evidence for peer effects, like an Apple enthusiast may primarily be friends with other Apple enthusiasts. So they develop **two instrumental variables** for the purchasing behavior of a person’s friends: the number of a user’s friends who randomly lose their phones, and the number of friends who have owned their phones for exactly two years, using NLP on Facebook de-identified data.

IV-2SLS.

