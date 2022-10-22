# Box-Office-Success

## Abstract
Movie production companies are interested in understanding what variables 
contribute to a successful film, particularly whether a film’s budget and IMBD score 
are predictive of net profits. Box office data from all 2019 film releases 
was collected and enhanced with additional features to address this question. 

Initially, a linear model was used to explore response associations and establish
a baseline. The initial model displayed poor fit according to the residual standard 
error distribution, warranting a more complicated analysis. Several hierarchical models
were used to address heteroscedastic variance concerns and ultimately a mixed effect
model was applied to observations based on release month which enhanced estimation 
accuracy for most fixed effects.

Final estimates for 'Budget' and 'Critic.Score' have significant positive effects 
on profitability at the 95% level. On average, every $1 increase in budget yields
an additional profit of $2.43 and improving the IMBD score by 1 point leads to a
net profit increase of ~$45 million. In addition, augmented field 'Title.Sentiment',
defined as the polarity score of the film's title, showed suprising significance,
indicating a ~$97 million net profit increase for every additional gain in sentiment
score. 

For production companies, it's not always feasible to create high budget, critically
acclaimed films, but they can control the naming. One actionable recommendation 
is to title movies positively, as audiences seem more inclined to purchase tickets
to these films.


## Documents of interest

- `Box-Office-Case-Study.pdf`: Written report, outlining our research, simulations procedure, case study, discussion, and results
- `Box-Office-Case-Study.Rmd` and `Scripts/` files: Code used to generate `Project.pdf`
- `./data/`: Raw data directory.
