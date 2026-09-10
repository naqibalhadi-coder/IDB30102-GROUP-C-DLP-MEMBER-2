# A-PANDDE: Advanced Provenance-based ANomaly Detection of Data Exfiltration

## Paper Information

**Title:** A-PANDDE: Advanced Provenance-based ANomaly Detection of Data Exfiltration

**Authors:** D. Fadolalkarim and E. Bertino

**Year:** 2019

**Publication:** Computers & Security, Volume 84, Pages 276–287

**DOI:** 10.1016/j.cose.2019.03.021

## Research Problem

The research addresses insider data exfiltration, particularly situations where authorised users may misuse legitimate access to organisational information.

## Method / Technique

A-PANDDE uses provenance-based anomaly detection to monitor user actions at the operating-system and file-system level. It creates user activity profiles and identifies unusual data-exfiltration behaviour.

The approach monitors activities such as database-to-file data flows, printing, emailing and copying.

## Dataset / Tools

The system was evaluated using a synthetic dataset in an Ubuntu virtual-machine environment.

## Main Findings

The approach demonstrates that monitoring the provenance of user and data activities can help identify anomalous data-exfiltration behaviour.

## Limitation

The implementation has limitations including dependence on PostgreSQL for certain database-related monitoring and the inability to track clipboard-copy activity.

## Relevance to Proposed Research

A-PANDDE supports the use of endpoint-level activity monitoring for detecting insider data exfiltration. This is relevant to the proposed DLP framework because the proposed solution also intends to monitor endpoint/process activity. However, the proposed research extends this approach by combining behavioural risk scoring with automated sensitive-data classification and DLP enforcement.
