# Statistical Inference Pipeline Demos (SIP-Demos)
This repo comes from my UCSD Math 189 notes, adapted from professor Siddharth Vishwanath in UCSD's math department. It involves many really good and intuitive visualzied demonstration of different `ideas in statistics`, which is really good for education purposes.

Non of the demos here are meant for an deep tour into all the mathamatical details in statistics, but rather a visual demonstartion of them and how to use them, which includes techniques that has theoritical roots in an arange of UCSD Math classes (Math 181A, Math 181B, Math 181E)

## Schematics 🧙‍♀️
Fundamentals:
- Covers basic linear algebra and probability that is important for statistics
    - **Linear algebra**: vectors/matrix, eigenvectors, solving linear systems
    - **Probability**: What is probability, PDF/CDF, all sorts of distribution families, expectation, variance, LLN, CLT
- Week1, week2, and week3 notebooks

Decision making (parametric):
- How do we make certain decisions when facing two alternative choices, we construct ideas from theroitical probability about how the world would look like under the hood if it is random (assuming LLN & CLT)
    - **Continuous random variable inference**: Confidence intervals, hypothesis tetsing, p-values, various test statistics
    - **Categorical random variable inference**: goodness of fit, test for independence, homogenity
    - **Moving towards more general form of testing**: MLE & likelihood ratio test
- Week3 and week4 notebooks

Decision making (non-parametric):
- How to make inference with minimal assumptions, we need a new paradigm starting from scratch
    - **Most naive non-parametric tests**:Wald-Wolfowitz runs test, KS-test
- Week5 notebook

Tetsing assumptions:
- Doe our assumption even make sense for us to do parametric test?
    - **Checking Independent + Identical**: QQ-plot, autocorrelation & Ljung-Box test
- Week5 and week6 notebook



Convert notebook by:

```bash
jupyter nbconvert --to pdf notebook.ipynb
```

Or use classic template by:

```bash
jupyter nbconvert --to html --template classic notebook.ipynb
```