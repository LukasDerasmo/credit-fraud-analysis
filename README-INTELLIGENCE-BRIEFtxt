Intelligence Brief
-     Develop a counter-fraud intelligence workflow to detect illicit financial patterns within a dataset of 284,807 European credit card transactions. Utilizing PCA-transformed features to maintain GDPR/PII compliance, the system identified $60,127 in fraudulent exposure across 492 confirmed cases. The investigation revealed distinct temporal attack vectors (late-night velocity spikes) and transaction structuring behaviors (averaging $122.21 per fraud instance vs. $88.29 for legitimate use), enabling targeted risk mitigation strategies.
  
Data Source & Anonymization Protocols
-     The dataset comprises 284,807 individual transactions in 2013 from European cardholders. To comply with privacy standards, the source data was subjected to anonymization before being published:
-     28 highly sensitive user features (e.g., identity, location, device telemetry) were mathematically transformed using Principal Component Analysis (PCA) into numerical vectors (V1 – V28). This preserves the statistical variance and correlation structures needed for pattern recognition while stripping away identifiers.
-     Absolute timestamps were removed and replaced with a "Time" delta (seconds elapsed since the initial dataset entry), allowing for time-based pattern analysis without revealing specific dates or individual user schedules.
-     Only two operational metrics, being Amount and Class (eg.- Fraudulent/Legitimate), were retained in their original format. Class takes the value of 1 in a case of fraud, 0 otherwise.

Operational Objectives
-     Architect a PostgreSQL data warehouse to manage raw transaction logs.
-     Apply statistical logic to masked PCA features to uncover hidden fraud vectors.
-     Deploy a Power BI operational dashboard to monitor financial exposure and fraud velocity.

Note
-     The dataset is highly unbalanced, the positive class (frauds) account for less than 1 percent of all transactions.
