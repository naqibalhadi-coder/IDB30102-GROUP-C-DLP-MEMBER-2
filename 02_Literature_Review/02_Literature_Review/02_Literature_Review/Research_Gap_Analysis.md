# Research Gap Analysis

## Identified Research Gap

The literature review identified three major research areas relevant to the proposed study: Data Loss Prevention (DLP), User and Entity Behavior Analytics (UEBA), and automated sensitive-data classification.

Existing DLP research demonstrates the ability to monitor data movement and enforce security policies. However, traditional or isolated DLP mechanisms may have difficulty distinguishing between legitimate and suspicious actions when an authorised user has valid access to sensitive information.

UEBA and insider-threat research addresses this problem from a behavioural perspective. User profiling, anomaly detection and dynamic risk scoring can identify activities that deviate from normal behaviour. However, behavioural anomalies alone do not necessarily indicate whether sensitive information is actually involved.

Automated data-classification research provides another important component by identifying sensitive information using machine learning, natural language processing and context-aware techniques. Nevertheless, these approaches generally focus on the characteristics of the data itself rather than the behavioural risk associated with the user performing the transfer.

## Gap in Existing Approaches

Based on the selected literature, there is limited integration of the following capabilities within a single adaptive enterprise DLP framework:

1. Endpoint and process activity monitoring.
2. UEBA-based dynamic user-risk scoring.
3. Automated context-aware sensitive-data classification.
4. Real-time DLP enforcement using both behavioural risk and data sensitivity.

This separation may contribute to false-positive alerts because a DLP system may make decisions without sufficient behavioural or contextual information.

## Proposed Research Direction

The proposed research addresses this gap through a multi-layered DLP framework in which endpoint activity, user behavioural risk and data sensitivity are evaluated together.

The proposed decision process is:

**User Activity → UEBA Risk Score → Data Classification → DLP Decision → Allow / Warn / Block**

For example, an authorised employee performing a normal transfer of non-sensitive information may receive a low-risk decision. In contrast, an employee exhibiting unusual behaviour while attempting to transfer highly sensitive documents may receive a higher combined risk assessment, causing the DLP system to warn or block the activity.

## Relationship to Research Objectives

**RO1:** Analyse existing DLP techniques and insider-threat detection methods to isolate current research gaps.

The literature review and comparison identify limitations in existing DLP, UEBA and data-classification approaches.

**RO2:** Design and develop a hybrid framework architecture integrating UEBA and automated context-aware data classification.

The identified integration gap provides the justification for combining these technologies within the proposed framework.

**RO3:** Evaluate the proposed solution's accuracy, recall and false-positive mitigation using test datasets.

The proposed framework can be compared with a baseline DLP approach to determine whether incorporating behavioural and contextual information improves detection while reducing false-positive alerts.
