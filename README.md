The repo looks great — all 5 files are in place! ✅

Now the last and most important step: **rewriting the README**. Let me write it for you right now based on your actual work.

Click the **pencil icon ✏️** on the README.md, select all the text, delete it, and paste this:

---

```markdown
# RCT Housing Mobility — Moving to Opportunity (MTO)

Causal analysis of the Moving to Opportunity (MTO) experiment using 
Intent-to-Treat (ITT) estimation and instrumental variables (Wald estimator) 
to measure the effect of housing voucher offers and relocation on 
psychological well-being.

## Background

The MTO demonstration, sponsored by the U.S. Department of Housing and Urban 
Development (HUD), was a randomized housing mobility experiment conducted 
between 1994 and 1998 across five U.S. cities: Baltimore, Boston, Chicago, 
Los Angeles, and New York. Low-income families in high-poverty public housing 
were randomly assigned to receive a housing voucher offer (experimental group) 
or remain without one (control group). This memo uses psychological distress 
(Kessler score) as the primary outcome.

## Key Results

| Estimand | Estimate | Interpretation |
|---|---|---|
| First Stage | +43.1 pp | Voucher offer → probability of moving |
| ITT | −0.588 Kessler pts | Voucher offer → psychological distress |
| TOT/LATE | −1.365 Kessler pts | Effect of moving for induced movers |

## Methods

- Randomized Controlled Trial (RCT)
- Intent-to-Treat (ITT) estimation
- Instrumental Variables / LATE (Wald estimator)
- Heteroskedasticity-robust standard errors (HC2)
- One-sided noncompliance (control-group moving ≈ 0)

## Repository Structure

```
rct_housing_mobility/
├── MTO_RCT.Rmd            # Full analysis: compliance, ITT, TOT/LATE
├── exhibits_mto.Rmd       # Exhibit charts for policy memo
├── mto_policy_memo.pdf    # Policy memo prepared for J-PAL audience
├── LICENSE
└── README.md
```

## Data

MTO public dataset via Harvard Kennedy School. Raw data (`mto.dta`) is 
not included in this repository. Contact HUD or NBER for access.

## Tools

R · tidyverse · haven · ggplot2 · sandwich · lmtest

## Author

Argenis Contreras · Harvard Kennedy School
