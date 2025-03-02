# Statistical Inference Pipeline Demos (SIP-Demos)
This repo comes from my UCSD Math 189 notes, adapted from professor Siddharth Vishwanath in UCSD's math department. It involves many really good and intuitive visualzied demonstration of different `ideas in statistics`, which is really good for education purposes.

Non of the demos here are meant for an deep tour into all the mathamatical details in statistics, but rather a visual demonstartion of them and how to use them, which includes techniques that has theoritical roots in an arange of UCSD Math classes (Math 181A, Math 181B, Math 181E)

## Schematics of SIP 🧑‍🔬

> ### Fundamentals 🔢
- Covers basic linear algebra and probability that is important for statistics
    - **Linear algebra**: vectors/matrix, eigenvectors, solving linear systems
    - **Probability**: What is probability, PDF/CDF, all sorts of distribution families, expectation, variance, LLN, CLT
- Week 1, week 2, and week 3 notebooks

> ### Decision making (parametric) 🤔
- How do we make certain decisions when facing two alternative choices, we construct ideas from theroitical probability about how the world would look like under the hood if it is random (assuming LLN & CLT)
    - **Continuous random variable inference**: Confidence intervals, hypothesis tetsing, p-values, various test statistics
    - **Categorical random variable inference**: goodness of fit, test for independence, homogenity
    - **Moving towards more general form of testing**: MLE & likelihood ratio test
- Week 3 and week 4 notebooks

> ### Decision making (non-parametric) 🤔
- How to make inference with minimal assumptions, we need a new paradigm starting from scratch
    - **Most naive non-parametric tests**:Wald-Wolfowitz runs test, KS-test
- Week 5 notebook

> ### Tetsing assumptions 🧪
- Doe our assumption even make sense for us to do parametric test?
    - **Checking for Independent + Identical**: QQ-plot, autocorrelation & Ljung-Box test woth autocorrelation
- Week 5 notebook

> ### Linear regression analysis (LRA) 📊
- How much can we learn by just fitting a line? What analysis can we drawn from fitting a line? What assumptions do we need to hold to run this analysis?
    - Different **interpretations** of LRA: optimization, correlation, probabilistic
    - Interpretations of **models and coefficients**
    - **Anatomy** of LRA (what you can get out of it): residuals, diffeernt sum of squares, $R$-squares, $F$-satistics, 
    - What **assumptions** do we need to hold to use LRA: independence, homestadasticity, noermality, linearity (notice, this is talking about the residuals, which is equivalence talking about the noices in teh probabilistci perspective)
    - Unusual observations in LRA
    - **More LRA**: categorical LRA, multi-dimensional LRA
- Week 6 notebook

> ### LRA coefficients tests 📊
- How can we do uncertainty quantification with this LRA that we have fitted? How can we utilize these coefficients that we have fitted?
    - Effects of **particular covaraiate**: individual coefficeint (linear hypothesis testing), analysis of varaince by making a smaller model (ANOVA), general linear hypothesis testing
- Week 7 notebook

> ### LRA interaction covariates 📊
- What happens when we have non-linear data and we may want to fit something that is more than linear?
    - We want to see **how much one thing change to effect the other**: Transformations, interaction terms and their theoritical constructs
    - **Too much** interactions: multicolinearity
- Week 7 notebook

> ### LRA Categorical responses 📊
- What if we don't wan to model a continuous response? Then LRA fails, we need to have a different way to formulate  model with LRA?
    - Modeling **odds**: logistics functions, interpretation of logistic coefficients (just like LRA), logistic assumptions, fitting logistic as for MLE for bernulli distribution
    - Logistci **in practice**: fit of logistic model (heuristic, confusion matrix, ROC), multi-nomial logistics
- Week 7 & 8 notebooks

> ### Variable selections 📊
- How doe we choose what variable to use? We can do ANOVA (this requires all possible subsets, this is not good computationally), but can we do something more general and more systematic?
    - **Selection criterions**: adjusted $R^2$ to number of predictors, AIC/BIC, and cross validation
    - **Stepwise selection**: forward, backward, and mix selection
    - **Shrinking methods**: anotehr perspective of regularizatin and shrinking
- Week 8 & 9 notebooks