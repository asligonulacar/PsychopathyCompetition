View Link: https://www.kaggle.com/c/twitter-psychopathy-prediction
# Description
The  aim of the competition is to determine to what degree it's possible to predict people with a sufficiently high degree of Psychopathy based on Twitter usage and Linguistic Inquiry.

The organizers provide all interested participants an anonymised dataset of users self assessed psychopathy scores together with 337 variables derived from functions of Twitter information, useage and lingusitc analysis. Psychopathy scores are based on a checklist developed by Professor Del Paulhus at the University of British Columbia.

The model should aim to identify people scoring high in Psychopathy, for the purpose of this competition, defined as 2 SD's above a mean of 1.98. This accounts for roughly 3% of the entire sample and therefore the challenge with this dataset is developing a model to work with a highly imbalanced dataset.

The best performing model(s) will be formally cited in a future paper/papers. The authors of the winning model may also be invited to attend future conferences to discuss their model.

# Evaluation
This competition uses "average precision", a metric which is more common for binary prediction but makes sense in this context as well. The true scores are sorted (descending) according to the order of the submission (only the order of the submission matters). In each row, we then compute the cumulative (from the top up to that row) "True Scores Ordered by Submission" divided by the cumulative "True Scores Ordered By True Scores", where that quotient is called the precision at row n. The final score is the average of the precision at row n (over all n).

