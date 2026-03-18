# ISP Business Analysis — Diagnostic & Descriptive Deep Dive

This project explores **customer churn, loyalty, billing pain points, and overage triggers** using a 300,000-row AI-generated synthetic dataset modeled on ISP’s service offerings.

---

##  Project Objective

To simulate and study the **current state of ISP's services and competitor benchmarks**, uncovering **opportunities for business improvements** in customer retention, loyalty growth, pricing friction, and churn prevention — with an aim to:

- Build a **360° view of customer lifecycle and friction**
- Discover **churn risk pockets** across credit, billing, plan design, and experience resolution
- Support **data-driven interventions** for loyalty reinforcement and revenue stabilization

---

##  Dataset Overview

This dataset is **synthetic and AI-generated**, designed to emulate realistic telecom subscriber behavior across key domains: billing, service usage, support events, loyalty tiering, and churn risk.

**Size:** 300,000 rows  
**Time Span:** Monthly snapshots across ~2 years  
**Built with:** AI generation + domain modeling of real telco features

### Key Columns & What They Mean

| Column              | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `Sub_ID`            | Unique subscriber ID                                                        |
| `Month_ID`          | Monthly snapshot of user activity                                           |
| `Total_Data_GB`     | Total data usage (WiFi + Cellular)                                          |
| `WiFi_Offload_Pct`  | % of data offloaded via WiFi networks                                       |
| `Cellular_Data_GB`  | Data consumed on cellular only                                              |
| `Bill_Amount`       | Final monthly bill charged                                                  |
| `Overage_Charge`    | Extra charge due to over-usage of data                                      |
| `Bill_Shock`        | Flag if bill amount significantly exceeds user norm                         |
| `Internet_Tenure_Mos` | Months since internet service started                                    |
| `Mobile_Tenure_Mos` | Months since mobile service started                                         |
| `Service_Bundle`    | User's service package: Mobile/TV/Internet combo                            |
| `Service_Count`     | Number of services subscribed                                               |
| `Rewards_Tier`      | Loyalty program status: None → Platinum                                     |
| `Line_Count`        | Number of mobile lines                                                      |
| `Zip_Code`          | User's service ZIP (for geo-segmentation)                                   |
| `Credit_Class`      | Financial profile: Prime, Subprime, No_Hit                                  |
| `Plan_ID`           | User’s subscribed plan (BTG_2025, UNL_PREM, etc.)                           |
| `Churn_Flag`        | Whether the user churned                                                    |
| `Churn_Reason`      | If churned, reason code (e.g., Activation_Failure, Bill_Shock)              |
| `Event_Type`        | Support or service-related events                                           |
| `Event_Outcome`     | Success/failure outcome of events                                           |
| `Resolution_Hrs`    | Time taken to resolve user-facing issues                                    |

---

## Analysis Phases

###  Descriptive Analysis

Key areas:

- Churn rate across **ZIP**, **bundles**, **credit class**, and **rewards tier**
- Revenue and overage trends across **line count**, **bundle size**
- Loyalty segmentation based on **tenure**, **service mix**, and **reward status**

>  Outcome: Identified top-performing cohorts and at-risk combinations based on revenue, friction, and churn.

###  Diagnostic Analysis

Root-cause discovery across:

- **Billing stress** (ARPU tiers, overage shocks)
- **Churn triggers** (plan type, credit profile, bill anomalies)
- **Resolution bottlenecks** (high `Resolution_Hrs` + low `WiFi_Offload_Pct`)
- Loyalty vs **friction** heatmaps (25-bin matrix across credit segments)

> Outcome: Segmented heatmaps + loyalty scoring models to enable precision retention targeting.

---

##  Business Value

| Area               | Actions                                                                 |
|--------------------|-------------------------------------------------------------------------|
| Churn Prevention | Multi-factor churn scoring using credit, friction, loyalty              |
| Plan Optimization| Recommend optimal plans based on usage, tenure, overage                 |
| Loyalty Growth   | Deploy segment-specific rewards and resolution SLAs                     |
| Support Strategy | Accelerate support for high-risk churners (Subprime, high-res time)     |
| Regional Control | Build ZIP-level dashboards to target onboarding and pricing hotspots    |

---

**[Aditya Nair]**  
adityanair1999@outlook.in  
GitHub: [github.com/AdityaNair-IND]  

---
