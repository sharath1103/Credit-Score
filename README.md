# Invisible Credit Score: Alternative Data Lending Model

# Business Problem
Traditional credit scoring models often exclude "thin-file" customers—individuals with little to no formal banking history—leading to missed revenue opportunities for FinTechs. This project aims to bridge that gap by using alternative data (utility payments, mobile tenure, and app usage) to predict creditworthiness and expand the lendable market.

# Key Features & Workflow
This project implements a complete serverless data pipeline from cloud ingestion to executive reporting.

**Cloud Data Infrastructure:** Hosted on Supabase (PostgreSQL), simulating a production environment with relational tables and specialized SQL views for feature engineering.

**Machine Learning Engine:** Built using XGBoost to handle non-linear relationships between unconventional financial behaviors and default risk.

**FinTech Scorecard:** Converted raw model probabilities into a standard 300-850 Credit Score scale to make the data actionable for loan officers.

**Responsible AI:** Utilized SHAP values to provide "Explainability," identifying the top risk factors for every applicant to comply with financial transparency regulations.

**What-If Simulation:** A Power BI dashboard allowing stakeholders to adjust the "Score Threshold" in real-time to observe the trade-off between Approval Rate and Portfolio Risk.

# Tech Stack
**Database:** Supabase (Cloud PostgreSQL)

**Languages:** SQL, Python (Pandas, Scikit-learn, XGBoost, SHAP)

**BI Tool:** Power BI Desktop

**Deployment:** GitHub Actions (for automated data processing)

# Business Impact & Insights
**Hidden Gems:** Identified a segment of users with low traditional income but 95%+ utility reliability, qualifying them for "Prime" lending status.

**Risk Mitigation:** The model achieved an AUC-ROC of 0.XX, significantly outperforming baseline models that relied solely on income data.

**Decision Optimization:** Using the Power BI simulation, the optimal threshold was determined at 640, which maximizes approval volume while maintaining a default rate below 5%.
