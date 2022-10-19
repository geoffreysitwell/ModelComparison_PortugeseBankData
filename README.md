# ModelComparison_PortugeseBankData

Credits for the data
[Moro et al., 2011] S. Moro, R. Laureano and P. Cortez. Using Data Mining for Bank Direct Marketing: An Application of the CRISP-DM Methodology. In P. Novais et al. (Eds.), Proceedings of the European Simulation and Modelling Conference - ESM'2011, pp. 117-121, Guimarães, Portugal, October, 2011. EUROSIS.

These data follow marketing campaigns from a Portugese banking institution. The aim of my project was to compare the accuracy and speed of a number of models and approaches in assessing whether customers would sign up for an account.

Because I do not use fixed states in my random test/train split I get slightly different results each time I run and so have decided to aggregate some of the results over 3 runs.

Summary Conclusions
Logistic Regression : Quite good results and doesn't seem to be  overfit due to similarity in train/test score
KNN                 : Same as Logistic Regression but much faster
Decision Tree       : Similar to KNN but seemingly ovefit due to perfect train score
SVC                 : Far too slow to be implemented. All of them greater than 70 minutes and is only marginally more accurate than assigning all as non-customers

Final Recommendation:
Decision Tree model is the preferred method for a combination of speed and accuracy. The model beats out a naive model and also executes quickly. Scaling comparisons indicate that maybe Decision Tree models will slow down with significantly more complicated datasets.
