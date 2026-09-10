Predicting Likelihood of Legitimate Data Loss in Email DLP

## Paper Information
**Title:** Predicting likelihood of legitimate data loss in email DLP

**Authors:** M. F. Faiz, J. Arshad, M. Alazab, A. Shalaginov

**Year:** 2020

**Publication:** Future Generation Computer Systems, Volume 110, Pages 744–757

**DOI:** 10.1016/j.future.2019.11.004

## Research Problem

Traditional Data Loss Prevention (DLP) systems can generate large numbers of alerts. Some alerts may represent legitimate data loss rather than malicious activity, making it difficult for security teams to prioritise incidents effectively.

## Method / Technique

The study applies machine learning techniques to historical email DLP incidents. Decision Tree and Random Forest models were investigated to predict the likelihood that a DLP incident represented legitimate data loss.

## Dataset / Tools

The researchers used historical email DLP incident data from a large UK telecommunications enterprise. The dataset contained 8,117 incidents.

## Main Findings

The Random Forest model achieved approximately 95% accuracy and around 90% true positive rate for predicting legitimate data loss.

Limitation

The research focuses specifically on email DLP incidents and prediction of legitimate data loss. It does not integrate user behavioural risk analysis with automated data sensitivity classification and endpoint enforcement.

## Relevance to Proposed Research

This study demonstrates that machine learning can help reduce the impact of DLP alert overload and improve incident prioritisation. It supports the proposed research objective of reducing false positives through intelligent analysis, while the proposed framework extends the idea by combining user behaviour analytics, data classification and DLP enforcement.
