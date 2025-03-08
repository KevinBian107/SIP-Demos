# Statistical Inference Pipeline Demos (SIP-Demos)
This repo comes from my UCSD Math 189 notes, adapted from professor Siddharth Vishwanath in UCSD's math department. It involves many really good and intuitive visualzied demonstration of different `ideas in statistics`, which is really good for education purposes.

None of the demos here are meant for an deep tour into all the mathamatical details in statistics, but rather a visual demonstartion of them and how to use them, which includes techniques that has theoritical roots in an arange of UCSD Math/Statistics classes (Math 181A, Math 181B, Math 181E)

## Schematics of SIP 🧑‍🔬
One key need for statsitical inference pipeline, different from both data analysis & machine learning, is that it needs to make predictions and inferences about th true population from looking at samples of it (unlike data analysis of just drawing conclusion) while maintaining the interpretability and understandability of it (unlike ML or DL). Hence, a major work in SIP is to constructs different forms of **assumptions** and **Interpretations** of the model.

> ### Fundamentals 🔢
- Covers basic linear algebra and probability that is important for statistics
    - **Linear algebra**: vectors/matrix, eigenvectors, solving linear systems
    - **Probability**: What is probability, PDF/CDF, all sorts of distribution families, expectation, variance, LLN, CLT
- Week 1, week 2, and week 3 notebooks

> ### Decision making (parametric) 🤔
- How do we make certain decisions when facing two alternative choices, we construct ideas from theroitical probability about how the world would look like under the hood if it is random (assuming LLN & CLT), then approach our testing statistics towards such distribution seeing if there is a significant differences between the reality sample and the theory.
    - **Continuous random variable inference**: Confidence intervals, hypothesis tetsing, p-values, various test statistics
    - **Categorical random variable inference**: goodness of fit, test for independence, homogenity
    - **Moving towards more general form of testing**: MLE & likelihood ratio test
- Parametric test will turns out to be very useful if we want to do test on LRA, which need assumptions to be hold, but if so, we can do a lot of tests to see teh significance of the coefficients.
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
    - Logistci **in practice**: fit of logistic model (heuristic, confusion matrix, ROC), multinomial logistics regression, interprettaion of multinomial logistic regression and marginal effects
- Week 7 & 8 notebooks

> ### Variable selections 📊
- How doe we choose what variable to use? We can do ANOVA (this requires all possible subsets, this is not good computationally), but can we do something more general and more systematic?
    - **Selection criterions**: adjusted $R^2$ to number of predictors, AIC/BIC, and cross validation
    - **Stepwise selection**: forward, backward, and mix selection
    - **Shrinking methods**: anotehr perspective of regularizatin and shrinking
- Week 8 & 9 notebooks

> ### Principal component analysis (PCA) 📚
- We have been doing supervised statistical inference for quite a while, but how do we find some interesting things when labels are not available?
    - **PCA Intuition**: deriving an optimization problem from statistical perspective and solving it with singular value decomposition
    - **Characteristic of PCA**: standardlize data PCA = covaraiate matrix PCA, addressing multicolinearity with principal component regression (PCR)
- Week 9 notebook

> ### Statsitical learning theory 🔢
- We will be looking at everything we have down from a more unifying perspective of statistical learning theory, this is also more familairily as **Empirical Risk Minimization (ERM)** used in most traditional machine elarning perspectives.
    - **Predictive intervals**: all of the previous model are creating manifolds on the data` by using parameter,can we test uncertainty on the predictions directly?
        - Confidence intervals of response in expectation
        - Prediction interval of individual response
    - **Statistical learning**
    - **Conformal inference**: Can we construct prediction/confidence indtervals for blackbox models?
- Week 10 notebook