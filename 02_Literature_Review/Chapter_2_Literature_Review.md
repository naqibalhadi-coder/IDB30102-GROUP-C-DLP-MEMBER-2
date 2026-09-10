# Chapter 2: Literature Review

## 2.1 Introduction

Data Loss Prevention (DLP) is an important security approach used to prevent sensitive organisational information from being disclosed, transferred or accessed inappropriately. Traditional DLP systems commonly rely on predefined policies, rules and signatures. Although these approaches can identify known patterns of sensitive information, they may generate large numbers of alerts and may not effectively detect insider threats involving legitimate users.

Recent research has explored machine learning, User and Entity Behavior Analytics (UEBA), provenance-based monitoring and automated data classification to improve data-loss prevention and insider-threat detection. The following literature review examines these approaches and identifies limitations that motivate the proposed multi-layered DLP framework.

## 2.2 Traditional DLP and Intelligent Alert Analysis

Faiz et al. (2020) investigated the prediction of legitimate data loss within email DLP environments. Their research applied Decision Tree and Random Forest machine-learning models to historical DLP incidents from a large telecommunications enterprise. The Random Forest model achieved approximately 95% accuracy, demonstrating that machine learning can assist in analysing DLP alerts and distinguishing potentially legitimate incidents.

However, the study is focused specifically on email DLP and the prediction of legitimate data loss. It does not combine user behavioural risk with automated classification of the sensitivity of the data being transferred. Therefore, additional behavioural and data-context information could potentially improve adaptive DLP decisions.

## 2.3 UEBA and Insider Threat Detection

Insider threats present a significant challenge because authorised users may misuse legitimate access. Khaliq et al. (2020) examined the role of User and Entity Behavior Analytics (UEBA) in detecting insider attacks. UEBA approaches establish behavioural profiles and identify deviations from expected user or entity activity. Risk-based analysis can help security teams identify suspicious behaviour.

Fadolalkarim and Bertino (2019) proposed A-PANDDE, a provenance-based anomaly detection approach for data exfiltration. The approach monitors user activities at operating-system and file-system levels and can analyse activities such as printing, emailing, copying and database-to-file data flows. This demonstrates the value of monitoring user activity and data movement at the endpoint level.

However, these approaches mainly focus on behavioural or activity-based anomaly detection. They do not provide a complete integration of behavioural risk with automated classification of the sensitivity and context of the data involved in the activity.

## 2.4 Automated and Context-Aware Data Classification

Automated classification can help identify sensitive information before a DLP decision is made. Guha et al. (2021) proposed a deep-learning model for information loss prevention from multi-page digital documents. Their approach used an MLP with n-gram TF-IDF features to classify documents. The research demonstrates how machine learning can support the identification of sensitive documents within large document collections.

Kužina et al. (2023) proposed CASSED, a context-based approach for structured sensitive-data detection. The method combines BERT with a rule-based layer and considers contextual relationships within and between cells and columns. This demonstrates the importance of context when identifying sensitive information rather than relying only on simple keyword or rule matching.

Muralitharan and Arumugam (2024) proposed Privacy BERT-LSTM for sensitive-information detection in textual documents. The approach combines BERT contextual embeddings with LSTM and attention mechanisms. The study demonstrates the potential of contextual NLP models for automated sensitive-information detection.

These studies demonstrate that automated classification can improve the identification of sensitive information. However, the reviewed classification approaches do not integrate user behavioural risk and real-time DLP enforcement into a single adaptive framework.

## 2.5 Comparison of Existing Approaches

The reviewed studies demonstrate that different techniques address different parts of the data-protection problem. Traditional and machine-learning-based DLP research focuses on improving alert analysis, while UEBA and provenance-based approaches focus on detecting abnormal user behaviour. Automated classification approaches focus on identifying sensitive information within documents or structured data.

The main limitation across the reviewed approaches is that these capabilities are generally investigated separately. A DLP decision could potentially become more adaptive if it considers both the user's behavioural risk and the sensitivity of the data involved.

## 2.6 Research Gap

Based on the reviewed studies, there is limited evidence within the selected literature of an integrated framework that combines:

1. Endpoint and process activity monitoring.
2. Dynamic UEBA-based user risk scoring.
3. Automated or context-aware sensitive-data classification.
4. DLP enforcement based on the combined risk and data sensitivity.

Existing studies provide strong individual components for these capabilities, but the reviewed approaches generally focus on one or two components rather than integrating them into a single adaptive DLP decision process.

Therefore, the proposed research aims to investigate a multi-layered DLP framework that combines user behavioural analysis and automated data classification. The proposed framework will use the relationship:

User Activity → UEBA Risk Score → Data Classification → DLP Decision → Allow / Warn / Block

This integration is intended to improve proactive data-loss prevention while reducing unnecessary alerts for legitimate activities.

## 2.7 Implications for the Proposed Research

The literature provides several design directions for the proposed framework. Endpoint activity monitoring can provide information about user actions and data movement. UEBA can convert behavioural information into a user-risk score. Automated classification can determine the sensitivity of the information involved in a transfer.

These components can then be combined within a DLP decision layer. For example, a low-risk user transferring non-sensitive information may be permitted, while a high-risk user attempting to transfer highly sensitive information may trigger a warning or blocking action.

This approach directly supports the research objectives by analysing existing techniques, designing an integrated framework and evaluating its ability to detect risky activity while reducing false positives.

## 2.8 Summary

The reviewed literature demonstrates that DLP, UEBA, anomaly detection and automated data classification can each contribute to enterprise data protection. However, the selected studies reveal a gap in integrating behavioural risk, data sensitivity and endpoint-level enforcement into one adaptive DLP framework. The proposed research addresses this gap by investigating a multi-layered framework that combines these capabilities to support proactive data-loss prevention and improved alert accuracy.
