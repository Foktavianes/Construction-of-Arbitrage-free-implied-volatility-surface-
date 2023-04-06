# Construction-of-Arbitrage-free-implied-volatility-surface-

The construction will address the several constraints that will lead to the condition of non-arbitrage. As long as the probability denstity exist, there will be no arbitrage in the implied vol surface. I start with this facts and address several conditions to address strike arbitrage and calendar arbitrage. I used cvxopt solver to find the value of strikes and densities that fit the conditions. After the construcion of implied volatility surface with basic requirements, I try to smoothen the surface with several trial and errors.
Lists of improvement techniques:
1. Implementation of weights matrix into the calculation using equal wieghtage and assigned weightage to certain areas.
2. Using second-order tikhonov regularization which add the penalty term to large change in curvature.
3. Integrate several boundary condition to address ITM and OTM area
