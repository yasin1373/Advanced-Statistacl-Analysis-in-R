# Blood Pressure Analysis with ANOVA in R
## Introduction

This project conducts analysis of variance (ANOVA) on a hypothetical blood pressure dataset to evaluate the impacts of treatment group and time on systolic blood pressure. Both mixed ANOVA and repeated measures ANOVA models are implemented in R to assess these effects while accounting for non-independence of observations over time within subjects.

## Methods

The blood pressure dataset contains repeated measurements of systolic blood pressure at baseline, week 1, and week 2 for subjects randomly assigned to a treatment or control group. 

Mixed ANOVA was performed using the lme4 package with time, group, and their interaction as fixed effects and subject as a random intercept. Repeated measures ANOVA was conducted with the rstatix package after reshaping to long format, with time, group, and their interaction as fixed effects and subject as the error term. 

Assumptions of normality, homogeneity of variance, and sphericity were checked prior to analysis. Post-hoc comparisons between time points and groups were carried out along with visualization of interactions.

## Results

The mixed and repeated measures ANOVA models yielded similar results, indicating a significant main effect of time on blood pressure, with reductions compared to baseline. The treatment group had significantly lower blood pressure than control overall. There was no significant time by group interaction.

## Conclusions

Both mixed and repeated measures ANOVA revealed significant declines in blood pressure over time as well as a treatment effect. The treatment intervention was effective at lowering blood pressure relative to control. The changes over time did not differ significantly between groups.

These methods demonstrate appropriate analysis of the longitudinal dataset using two approaches to ANOVA with non-independent observations. The R code provides a template for implementing both mixed models and reshaping data for repeated measures.

