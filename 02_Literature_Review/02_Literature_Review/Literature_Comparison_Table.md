# Literature Review Comparison Table

| Study | Research Focus | Method / Technique | Dataset / Environment | Main Findings | Limitation |
|---|---|---|---|---|---|
| Faiz et al. (2020) | Email DLP and alert analysis | Decision Tree and Random Forest | 8,117 historical email DLP incidents from a UK telecommunications enterprise | Random Forest achieved approximately 95% accuracy and around 90% true-positive rate | Focused on email DLP and does not integrate user behaviour with sensitive-data classification |
| Fadolalkarim & Bertino (2019) | Insider data exfiltration | Provenance-based anomaly detection and user activity profiling | Synthetic dataset in an experimental environment | Demonstrated detection of anomalous activities involving copying, printing, emailing and data movement | Focused on specific provenance and file-system scenarios; limited integration with content classification |
| Khaliq et al. (2020) | Insider-threat detection | UEBA, behavioural profiling and risk scoring | UEBA-focused study; no single experimental dataset identified in the reviewed information | Shows how behavioural profiles and risk scores can support insider-threat detection | Behavioural analysis does not determine the sensitivity of the data being transferred |
| Guha et al. (2021) | Sensitive document classification | MLP with n-gram TF-IDF features | Large enterprise digital-document environment | Demonstrated automated classification of sensitive and non-sensitive documents | Focuses on document classification without dynamic user-risk analysis |
| Kužina et al. (2023) | Context-aware sensitive-data detection | BERT combined with a rule-based layer | Structured sensitive-data datasets | Contextual information improved sensitive-data detection | Focuses mainly on structured/tabular data and does not incorporate UEBA |
| Muralitharan & Arumugam (2024) | Sensitive information detection | BERT-LSTM with attention | SMS Spam Collection dataset | Reported 92.50% accuracy, 89.36% precision and 85.02% F1-score | Dataset is not representative of a full enterprise DLP environment and no UEBA/DLP enforcement is integrated |

## Overall Comparison

The reviewed studies can be divided into three main areas:

- **DLP and alert analysis:** Faiz et al. (2020)
- **UEBA and insider-threat detection:** Fadolalkarim and Bertino (2019); Khaliq et al. (2020)
- **Automated sensitive-data classification:** Guha et al. (2021); Kužina et al. (2023); Muralitharan and Arumugam (2024)

The comparison indicates that existing research provides useful techniques for individual layers of enterprise data protection. However, within the selected literature, limited integration is observed between dynamic user-risk analysis, context-aware sensitive-data classification and real-time DLP enforcement.

## Comparison With Proposed Framework

| Capability | Existing DLP Research | UEBA Research | Data Classification Research | Proposed Framework |
|---|---|---|---|---|
| Sensitive data detection | Yes | Limited | Yes | Yes |
| User behaviour monitoring | Limited | Yes | No | Yes |
| Dynamic user risk scoring | Limited | Yes | No | Yes |
| Context-aware classification | Limited | No | Yes | Yes |
| Endpoint/process monitoring | Varies | Yes | Limited | Yes |
| DLP enforcement | Yes | Limited | No | Yes |
| Combined multi-layer decision | Limited | Limited | Limited | Yes |

The proposed framework therefore aims to combine capabilities that are commonly treated independently by existing approaches.
