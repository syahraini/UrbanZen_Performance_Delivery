# UrbanZen Delivery Performance Analytics - Project Brief

## 1. Project Overview

This project analyzes UrbanZen's delivery operations using 200,000+ e-commerce transaction records, including delivery timestamps, customer satisfaction scores, seller performance data, and geographic information.

The goal is to identify root causes of delivery delays, quantify their impact on customer satisfaction, and provide actionable insights to improve operational efficiency.

---

## 2. Business Objectives

- **Primary:** Identify and quantify the relationship between delivery performance and customer satisfaction
- **Secondary:** Pinpoint seller-specific performance issues and geographic patterns
- **Strategic:** Develop data-driven recommendations to reduce delays and improve customer experience

**Key Business Questions:**

1. How often does UrbanZen deliver late?
2. What is the correlation between delays and customer satisfaction?
3. Which sellers/regions contribute most to delivery issues?
4. How severe are the delays when they occur?
5. What is the financial/reputational impact of current performance?

---

## 3. Scope & Boundaries

### Included:

- Delivery timeliness analysis (on-time vs. delayed)
- Customer satisfaction correlation studies
- Seller performance segmentation and tiering
- Geographic delay pattern analysis
- Operational KPI development and tracking

### Out of Scope:

- Forecasting future delivery performance
- Customer demographic profiling
- Competitor benchmarking analysis
- Cost impact and ROI calculations
- Real-time monitoring system implementation

---

## 4. Data Sources & Architecture

| Data Domain | Record Count | Key Fields |
| --- | --- | --- |
| Full Delivery Table | 200,000+ | order_date, estimated_date, delivered_date, seller_id, order_id, rating, seller_location, region |

**Data Quality Notes:**

- Timestamp consistency required validation across systems
- 2.1% of records excluded due to incomplete delivery information

---

## 5. Stakeholders & Responsibilities

| Role | Primary Responsibility | Engagement Level |
| --- | --- | --- |
| **Head of Operations** | Strategic decision-making, budget approval | High |
| **Customer Experience Manager** | Insight application, process improvements | High |
| **Vendor Relationship Manager** | Seller performance management | Medium |
| **Data Analyst (Project Lead)** | End-to-end analysis, dashboard development | High |
| **IT/Data Engineering** | Data extraction and pipeline support | Low |

---

## 6. Analytical Approach

### Phase 1: Data Foundation

- **Data Extraction:** SQL queries to extract and merge transactional data
- **Data Cleaning:** Handle missing timestamps, standardize ratings, validate seller IDs
- **Feature Engineering:** Calculate delay flags and delay duration

### Phase 2: Exploratory Analysis

- **Correlation Analysis:** Delivery timeliness vs. customer satisfaction
- **Segmentation Analysis:** Seller performance clustering
- **Trend Analysis:** Monthly/quarterly performance patterns
- **Geographic Analysis:** Regional delay concentration for both customer and seller

### Phase 3: Insight Development

- **Root Cause Identification:** Pareto analysis of delay drivers
- **Impact Quantification:** CSAT score differentials by delay severity
- **Opportunity Sizing:** Potential improvement from addressing worst performers

### Phase 4: Dashboard & Reporting

- **Tableau Development:** Interactive operational dashboard
- **Executive Summary:** Key findings and recommendations
- **Action Plan:** Prioritized improvement initiatives

---

## 7. Key Performance Indicators (KPIs)

| KPI | Definition | Target |
| --- | --- | --- |
| **On-Time Delivery Rate** | % of orders delivered by promised date | >95% |
| **Average Delay Duration** | Mean days late for delayed orders | <3 days |
| **CSAT Impact Score** | Rating difference: on-time vs. delayed | <0.5 point drop |
| **Seller Performance Tier Distribution** | % of sellers in each performance category | 80% in Tier 1 |
| **Regional Delay Concentration** | Gini coefficient of delays by region | <0.3 |

---

## 8. Deliverables

### Core Deliverables:

- Interactive Tableau Dashboard (Operational View + Executive Summary)
- SQL Data Transformation Scripts
- Comprehensive Analysis Report (PDF)

### Supporting Materials:

- Project Methodology Documentation
- Stakeholder Presentation Deck

---

## 9. Success Metrics

- **Analytical Success:** Clear identification of 3+ root causes with data-backed evidence
- **Business Success:** Stakeholder approval of recommended action plan
- **Operational Success:** Dashboard adoption by operations team for weekly reviews
- **Impact Success:** 15% reduction in delay rates within 3 months of implementation

---

## 10. Tools & Technology Stack

| Category | Tools |
| --- | --- |
| **Data Processing** | SQL, Microsoft Power Query |
| **Analysis & Visualization** | Tableau, Excel |
| **Documentation** | Notion |
| **Project Management** | Notion |
| **Version Control** | GitHub (for SQL scripts and documentation) |

---

## 11. Risks & Mitigations

| Risk | Impact | Mitigation Strategy |
| --- | --- | --- |
| Data quality issues | High | Early data profiling, exclude unreliable segments |
| Stakeholder availability | Medium | Bi-weekly checkpoints, clear documentation |
| Scope creep | Medium | Strict adherence to defined boundaries, change log |
| Technical limitations | Low | Prototype early, validate tool capabilities |

---

*Document Version: 1.0 | Last Updated: 2025, November 29 | Owner: Syahraini*