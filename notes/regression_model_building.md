### Building Models

- You need to be able to remove or limit variables/predictors that aren't contributing to the outcome. Otherwise your model would be representing to generally without providing concrete cause -> effect.

#### Backward Elimination

- Step 1: Select a Significance Level (SL) to stay in the model (like SL = 0.05)
- Step 2: Fit the full model with all possible variables/predictors
- Step 3: Consider the predictor with the highest P-Value. If P > SL, go to step 4, otherwise go to Done
- Step 4: Remove the predictor/variable that is high-P
- Step 5: Fit model without this variable/predictor _(REPEAT -> Step 3)_
- Note: Once you remove a noisy or insignificant predictor/variable, you will need to completely rebuild the model because the effects of the whole will be altered when any one is removed.

#### Forward Selection

- Step 1: Select a Significance Level (SL) to _enter_ the model (e.g. SL = 0.05).
- Step 2: Fit all simple regression models $y = x_n$ Select the one with the lowest P-value
- Step 3: Keep this variable and fit all possible models with one extra predictor added to the one(s) you already have.
- Step 4: Consider the predictor with the lowest P-value. If P < SL, go to Step 3 (repeat), otherwise go to FIN (final)

#### Bidirectional Elimination (Combines previous 2 methods) (a.k.a Stepwise Regression )

- Step 1: Select a Significance Level (SL) to _enter_ _and_ to _stay_ in the model (e.g. SL_ENTER = 0.05, SL_STAY = 0.05)
- Step 2: Perform steps from Forward Selection (new variables must have P < SL_ENTER to enter)
- Step 3: Perform ALL steps of Backward Elimination (old variables must have P < SL_STAY to stay)
- Step 4: No new variables can enter and no old variables can exit

#### All Possible Models

- Step 1: Select a criterion of goodness of fit (e.g. Akaike criterion)
- Step 2: Construct all possible regression models: $2^n - 1$ total combinations
- Step 3: Select the one with the best criterion
- Note: Example having 10 columns would mean 1,023 models .. Even though this would be the most 'thourough' method, it is extremely expensive.
