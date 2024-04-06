# PLUS ADVISORY

_"Insert Quote" - Benjamin Franklin_

---
>
* Click [link](https://classroom.github.com/a/biNKOeX_) to accept your group assignment.

When you finish the task, please paste your link to the Excel [sheet](https://unsw-my.sharepoint.com/:x:/g/personal/z5096423_ad_unsw_edu_au/ETIxmQ6pESRHoHPt-PUleR4BuN0_ghByf7TsfSfgDaBhVg?rtime=GAd2OFNM3Eg) for Peer Feedback
---
>Be creative! Feel free to link to embed your [data](2024-srcsc-superlife-inforce-dataset-part1.csv), [code](sample-data-clean.ipynb), [image](unsw.png) here


## Problem Statement
SuperLife, a prominent life insurance carrier in the country of Lumaria, is exploring the development of a health incentive program to complement its long-term life insurance products. Through the health program, Superlife seeks to incentivize healthy lifestyle behaviours and thereby decrease policyholder mortality rates, and boost sales volumes via enhanced marketability and industry competitivenes to ultimately yield economic benefits for the company. Plus Advisory has been engaged as an external consultancy to propose an innovative solution.

## Executive Summary
This showcase presents Plus Advisory’s proposed ‘wellness plan’ with detailed examination into the program design, modelling and evaluation process. These investigations were commissioned by *SuperLife Chief Actuary Jes B. Zane* to address several strategic social, financial and growth objectives for SuperLife’s long-term life insurance products. Included below is a comprehensive review of the initial data exploration, our health program design process, assumptions setting procedure, pricing-model construction methodology and forecasted economic benefits until 2044. To assess and support the long-term financial viability and profitability of the health program, sensitivity analyses and risk evaluations were also conducted. In recommending implementation of the health plan, there are further discussions of other considerations such as using gender-based pricing and devised marketing plans across Lumaria.

## Project Timeline
The chart below depicts the workflow progression of Plus Advisory's consultants in developing the solution.
> Project Timeline

![Timeline (1)](https://github.com/Actuarial-Control-Cycle-T1-2024/group-page-showcase-cc2024/assets/166011854/4132fb2e-3e7f-4265-85b9-f3149fec1b2d)

## EDA

## Assumptions
### Expenses

![Expenses](https://github.com/Actuarial-Control-Cycle-T1-2024/group-page-showcase-cc2024/assets/166011854/aaf64308-2d2e-45f6-b5bd-6e55e23445fe)


### Earnings on Investment Rate and Net Investment Income Allocation

![Investment Allocation](https://github.com/Actuarial-Control-Cycle-T1-2024/group-page-showcase-cc2024/assets/166011854/a08a7b36-6e93-44eb-9b47-9347a5ef5208)

### Lapse Rate
* Assume that only T20 policies have lapses and SPWL does not because policyholders aren't likely to lapse after paying the single premium at the start of the policy.
* All future lapse rates are consistent with the historical trend

Lapse rates of each policy year durations were calculated using the following formula:

<img width="250" alt="Screenshot 2024-04-06 at 10 10 47 pm" src="https://github.com/Actuarial-Control-Cycle-T1-2024/group-page-showcase-cc2024/assets/165151626/8d394cfa-6ba8-4f20-8e9c-962feb6e9888">

<ins>Method<ins>
1. Created new column that calculated Years to Lapse (how long it took for each lapsed policyholder to lapse) and counted frequencies from 0 to 19
2. Calculated number of in force policies e.g. how many not dead or lapsed in 2001 when policy issued in 2001, how many not dead or lapsed in 2002 when policy issued in 2002.... which summed to ALL active
3. Repeated until Policy Year 19

> Lapse Rate Trend for T20
<img width="550" alt="Screenshot 2024-04-06 at 11 40 12 pm" src="https://github.com/Actuarial-Control-Cycle-T1-2024/group-page-showcase-cc2024/assets/165151626/6add8821-581f-4a77-a464-7439e62e4bca">

**Values are recorded in this [lapse rate table](LapseRate.png)*



### Inflation Rate

### Discount Rate

### Mortality Rate

### New Business Volume

![New Business Volume](https://github.com/Actuarial-Control-Cycle-T1-2024/group-page-showcase-cc2024/assets/166011854/5add1704-f32e-4a5c-a7f9-d83778a9ee86)

### New Business Demographics

![SPWL Demo](https://github.com/Actuarial-Control-Cycle-T1-2024/group-page-showcase-cc2024/assets/166011854/ad598bd3-4a66-4635-b996-a6bea1fa31b0)
![T20 Demo](https://github.com/Actuarial-Control-Cycle-T1-2024/group-page-showcase-cc2024/assets/166011854/98825cd0-c0f2-4670-a221-287adf794ac5)

## Risk Management
Significant quantitative and qualitative risks that may arise from the implementation of the health incentive program for SuperLife were identified and assessed. For each risk, ratings of the magnitude of impact and the possibility of occurrence are provided in this [risk matrix](Likelihood.png), alongside relevant mitigation strategies deduced to address these risks, outlined in the table below.

> Risks and Mitigation Strategies

![Screenshot 2024-04-05 at 8 42 48 pm](https://github.com/Actuarial-Control-Cycle-T1-2024/group-page-showcase-cc2024/assets/165151626/9731c6ef-58f1-4502-be90-ccf12f5fdcb1)

### Sensitivity Analysis
Sensitivity analysis was conducted to assess the materiality of the financial impacts from favourable and unfavourable scenarios based on our key assumptions. The table below details the different scenarios investigated, the recommended range that our health plan will remain financially viable within and any insights gathered during the analysis.

> Sensitivity Testing - Scenarios, Impacts and Insights

![Sensitivity Analysis Table](https://github.com/Actuarial-Control-Cycle-T1-2024/group-page-showcase-cc2024/assets/165151626/5d36d746-417d-43d1-98c7-21b328d39f65)
