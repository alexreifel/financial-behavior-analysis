# Financial Behavior Analysis

How accurately do people understand their own financial knowledge — and does the gap between confidence and competence show up in real financial behavior?

This project analyzes the relationship between **financial confidence**, **financial competence**, and **financial well-being** using the 2024 National Financial Capability Study (NFCS) State-by-State Survey, covering approximately 25,500 U.S. adults.

Completed for the NYU Data Science Club Project Expo by **Makaila Kim, Alex Reifel, and Rebecca Wang**.

## Research Questions

1. How closely does self-reported financial confidence match actual financial literacy?
2. How do overconfident and underconfident individuals differ in financial well-being?
3. Can observable financial behavior predict someone's confidence or competence?

## Methodology

We measured:

- **Financial confidence** using respondents' self-assessed financial knowledge.
- **Financial competence** using performance on the NFCS "Big Five" financial literacy questions.
- **Financial well-being** using measures related to spending, emergency savings, debt, credit, retirement planning, and financial stress.

Respondents were segmented into four groups:

- Realistic-Low
- Underconfident
- Overconfident
- Realistic-High

We then compared financial outcomes across these groups and trained Random Forest classifiers using financial-behavior variables to predict high versus low confidence and competence.

## Key Findings

- Confidence and competence frequently do not align.
- Underconfidence appeared more common than overconfidence in our segmentation and was associated with meaningful differences in financial well-being.
- Observable financial behavior predicted **financial competence slightly better than financial confidence**.
- The Random Forest models achieved approximately **62% accuracy for confidence** and **64% accuracy for competence**, correctly classifying roughly two out of three respondents.
- Important predictors of competence included retirement-planning behavior, emergency savings, and the ability to raise $2,000 in an emergency.
- Important predictors of confidence included confidence in achieving financial goals, time spent worrying about finances, and self-rated credit quality.

One takeaway from the modeling was that competence is more directly tied to observable saving and planning behavior, while confidence also reflects harder-to-observe factors such as self-perception and bias.

## Files

### Code

The Jupyter notebook contains the full data-cleaning, segmentation, visualization, and modeling workflow.

[View Notebook](Mind%20over%20Money%20Code.ipynb)

### Presentation

The final presentation summarizes the methodology, findings, model results, and implications.

[View Slides](https://docs.google.com/presentation/d/1K9PPipWEeG8vXazGf8P_3u3Pns4dnLAkFmqcafw91jI/edit?usp=sharing)

## Tools

Python · pandas · NumPy · scikit-learn · Random Forest · Matplotlib · seaborn
