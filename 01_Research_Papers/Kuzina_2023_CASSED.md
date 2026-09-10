# CASSED: Context-based Approach for Structured Sensitive Data Detection

## Paper Information

**Title:** CASSED: Context-based Approach for Structured Sensitive Data Detection

**Authors:** V. Kužina, A.-M. Petric, M. Barišić, and A. Jović

**Year:** 2023

**Publication:** Expert Systems with Applications, Volume 223, Article 119924

**DOI:** 10.1016/j.eswa.2023.119924

## Research Problem

Sensitive information can be difficult to identify accurately when its meaning depends on the context in which it appears. Simple keyword or rule-based approaches may not adequately understand relationships between data fields.

## Method / Technique

CASSED combines a BERT-based language model with a rule-based layer to detect sensitive information using contextual relationships within and between cells and columns.

## Dataset / Tools

The researchers evaluated the approach using existing datasets together with a newly created dataset containing structured sensitive data.

## Main Findings

The study demonstrates that incorporating contextual information can improve the detection of sensitive data in structured datasets compared with approaches that rely less heavily on context.

## Limitation

CASSED focuses primarily on structured or tabular data. It does not incorporate user behavioural analysis or endpoint-level DLP enforcement.

## Relevance to Proposed Research

CASSED supports the proposed use of context-aware automated data classification. It demonstrates why identifying sensitive data based only on simple static rules may be insufficient. The proposed framework extends this concept by combining data sensitivity with UEBA-based user risk and DLP enforcement.
