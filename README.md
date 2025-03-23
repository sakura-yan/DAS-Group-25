# Spam Email Classification Analysis

## Dataset Information
Dataset 25 was collected by Hewlett-Packard Labs and shared with the UCI Machine Learning Repository. These dataset contains data about classifying emails as spam or not spam, with extra information showing the frequency of certain words and characters in the email.

### Variables:
- **crl.tot** – The total length of uninterrupted sequences of capital letters.
- **dollar** – The percentage of the total number of characters that are dollar signs (`$`).
- **bang** – The percentage of the total number of characters that are exclamation marks (`!`).
- **money** – The percentage of the total number of characters that are the word "money".
- **n000** – The percentage of the total number of characters that are the string "000".
- **make** – The percentage of the total number of characters that are the word "make".
- **yesno** – A variable that shows if the email was spam (`y`) or not spam (`n`).

## Research Objective
The goal of this analysis is to find the features in spam emails that can improve the company’s spam email filter.

### Research Question:
**What text features influence whether an email is classified as spam or not?**

## Methodology
To answer this question, a **Generalized Linear Model (GLM)** with logistic regression was used. This model looks at the relationship between email features and whether an email is spam. Several transformations and binning techniques were applied to improve the model’s performance.

## Files Included
- **`Group_25_Analysis.qmd`** – The Quarto Markdown file that contains the analysis and model development.
- **`Group_25_qmd.pdf`** – The PDF document generated from the Quarto file.
- **`Group_25_Presentation.pptx`** – A PowerPoint presentation with the main findings.
- **`dataset25.csv`** – The dataset used for the analysis.

## Key Findings
- **Financial symbols** such as dollar signs (`$`) and the word "money" are strong indicators of spam.
- **Exaggerated punctuation**, particularly exclamation marks (`!`), is commonly seen in spam emails.
- **Anomalous patterns**, such as long sequences of capital letters and repeated "000", are associated with spam emails.
- The term **"make"** is often found in non-spam emails, suggesting it may be a feature more common in legitimate content.
  
These findings highlight the importance of certain patterns and words in identifying spam. Specifically, the presence of financial symbols, exaggerated punctuation, and anomalous patterns like capital bursts and "000" are strong indicators of spam. In contrast, terms like "make" may signal non-spam contexts.

## Conclusion
This analysis provides key insights into which features are most relevant for detecting spam emails. The findings can be used to enhance spam filtering systems by targeting these specific text characteristics.


