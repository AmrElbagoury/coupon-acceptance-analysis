# Will a Customer Accept the Coupon?

## Overview
The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

## Dataset
- **Source:** UCI Machine Learning Repository via Amazon Mechanical Turk
- **Size:** 12,684 observations and 26 features
- **Coupon Types:** Bar, Coffee House, Carry Out & Take Away, 
  Restaurant (under $20), Restaurant ($20-$50)

## Key Findings

### Bar Coupons
* **Frequency of bar visits is the strongest predictor of acceptance.** Drivers who visit bars more than 3 times a month accepted at nearly double the rate (**76.88%**) compared to those who go 3 or fewer times (**37.07%**).
* **Social context matters more than age.** Drivers who go to bars more than once a month without kids as passengers accepted at **71.79%**, while adding the age filter (over 25) slightly reduced the rate to **69.52%**.
* **Occupation play a role.** Removing drivers in farming, fishing, and forestry occupations from the frequent bar-goer group maintained a high acceptance rate of **71.79%**
* **Budget-conscious drivers are less likely to accept bar coupons.** Group 3 (cheap restaurant goers with income under $50K) had the lowest acceptance rate at **45.35%**, suggesting that cost-conscious drivers may not see bar coupons as aligned with their spending habits even if they dine out frequently.
* **The combined group still outperforms all others.** The combined group acceptance rate of **56.93%** versus **33.19%** for all others confirms that these lifestyle and behavioral factors together are meaningful predictors of bar coupon acceptance

### Coffee House Coupons
* **Younger drivers are the most receptive audience..** rivers `below21` had the highest acceptance rate at **69.68%**, nearly 20 points above the `50plus` group (**42.02%**). When combined with `Friend(s)` as passengers,this group reached an exceptional **85.37%** acceptance rate.
* **Destination matters.** Drivers with no urgent destination accepted at **58.10%**, nearly 22 percentage points higher than those heading `Home` (**36.21%**. 
* **Longer expiration windows drive higher acceptance.** Coupons expiring in `1d` achieved a **58.39%** acceptance rate versus only **43.20%** for `2h` coupons.
* **Combining favorable conditions significantly boosts acceptance.** The combined group of young drivers `below21` with `Friend(s)` who were offered coupons expiring in `1d` achieved **90.91%** acceptance rate versus **41.21%** for all others.

## Recommendations
- **Bar coupons** Drivers who already frequent bars, travel without children, and work in non-agricultural occupations are the most likely to accept bar coupons.
- **Coffee house coupons** Coffee house coupons are most likely to be accepted by drivers under 21 traveling with friends, during morning or early afternoon hours, with no urgent destination, and with a full day to redeem the coupon.


## Tools Used
- Python, Pandas, Matplotlib, Seaborn, Numpy Jupyter Notebook

## Links
- [Jupyter Notebook](https://github.com/AmrElbagoury/coupon-acceptance-analysis/blob/main/coupon_acceptance_analysis.ipynb)