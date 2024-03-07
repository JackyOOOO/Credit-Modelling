This is the implementation of the CERM model.

Objective: Estimate credit losses per year given a scenario with multi factors (e.g., Economic condition, Climate, Other impacts)

Input:
1. Exposure of the portfolio
2. Loss Given Default (LGD)
3. Transition Matrix (Probability of the rating migrate to the other rating/stay in the same rating)
4. Factors representing the condition (from ytd to year n)
5. Correlation Matrix (C)

Output:
Loss distribution per year

Possible Usage:
Calculate 1. Expected loss, 2. Unexpected loss/RWA, 3. Reverse Stress test


Explanation:

1. Use Gaussian Copula Model to model the asset value (X)
  <img width="315" alt="Screenshot 2024-03-07 at 9 09 53 PM" src="https://github.com/JackyOOOO/Credit-Modelling/assets/106862996/f211086f-5f6a-4233-be87-953d987e5c6d">

2. 
<img width="408" alt="Screenshot 2024-03-07 at 9 16 54 PM" src="https://github.com/JackyOOOO/Credit-Modelling/assets/106862996/4a1a9eb3-93b9-468b-994f-f740448ff9c7">
