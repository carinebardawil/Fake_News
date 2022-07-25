# Fake_News
Valital Technologies Technical Test
By Badr Ouazou & Keywan Esfahani
We want to do fact checking on news data with the DataCommons FactCheck dataset. 
 
Dataset
You can easily access this dataset with the HuggingFace (HF) datasets library: 
 
https://huggingface.co/datasets/datacommons_factcheck
 
You load it like this:
 
from datasets import load_dataset
 
dataset = load_dataset("datacommons_factcheck", "fctchk_politifact_wapo")
 
 
Use the fctchk_politifact_wapo version.
 
Label
There are many labels in the review_rating column, but we would like a binary approach: the information in the news is a FAKE NEWS or a TRUE NEWS.
 
It is up to you as an nlp scientist to group the original classes accordingly. 
 
Hint: you can filter out very rare classes with few occurrences.

Use Case
Consider that we want to review a list of fake news every day to report them to their respective publishers, but we are a small team and cannot review every flagged news. We would like you, the nlp scientist, to build a model to classify fake news or not, then, one content moderator on the team will check the predictions.
 
 

Questions
 
What is your overall methodology from data gathering to producing that list of fake news? 
Please also explain the goal of every step. 
steps: exploration, training and inferencing.
Explain your modeling approach (features, model, output tuning) and all the improvements.
With all the considerations in this use case, what metric should we use (ie: accuracy, precision, recall, F-1 score…)? Why?
What are the mistakes made by your model? Are there any patterns?
What are the next steps to improve this use case?

Technical tips
Use a GIT repository (that you can share with us for the submission).
Use the HuggingFace datasets loading function (refer to Dataset part) for easier reproducibility.
Consider technical aspects: 
Code readability (clean, meaningful comments, project structure, typing, etc.)
Code refactoring and testing
Optimization
Good practices of git (commits, branching, etc.)
Documentation
Submission
The deadline is Monday July 25 2022 at 11 pm. 
Send an email to badr.o@valital.com & mingyou.s@valital.com containing your technical test:

GitHub repository link.
Slides or a report where you present your approach and your results (with answers to questions).


