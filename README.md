# Hypothesis Analysis and A/B Testing for an Online Store

This project analyzes marketing hypotheses and A/B test results for a large e-commerce company. The goal is to identify growth opportunities, increase revenue, and make data-driven decisions based on hypothesis frameworks and statistical evaluation.

## 📌 Project Goals

- Prepare and prioritize a list of hypotheses aimed at increasing revenue.
- Apply ICE and RICE frameworks for prioritization.
- Launch and analyze the results of an A/B test.
- Identify anomalies in user behavior and orders.
- Make informed business decisions based on statistical evidence.

## 🧭 Workflow

1. **Data Overview & Cleaning**
2. **Hypothesis Prioritization**
   - ICE (Impact, Confidence, Effort)
   - RICE (Reach, Impact, Confidence, Effort)
3. **A/B Test Analysis**
   - Cumulative metrics (revenue, average order value, conversion)
   - Relative changes between test groups
   - Detection of anomalies (outliers in orders and revenue)
   - Statistical significance testing (raw vs. filtered data)
4. **Final Recommendation**
   - Conclude whether to stop or continue the test based on metrics.

## 📂 Data Description

### 1. Hypotheses (`hypothesis.csv`)
| Column       | Description                                  |
|--------------|----------------------------------------------|
| Hypothesis   | Brief description of the hypothesis          |
| Reach        | Estimated user reach (1–10)                  |
| Impact       | Expected impact on users (1–10)              |
| Confidence   | Confidence in hypothesis success (1–10)      |
| Efforts      | Resource cost to test the hypothesis (1–10)  |

### 2. Orders (`orders.csv`)
| Column         | Description                                |
|----------------|--------------------------------------------|
| transactionId  | Unique order ID                            |
| visitorId      | Unique user ID                             |
| date           | Order date                                 |
| revenue        | Order revenue                              |
| group          | A/B test group (A or B)                    |

### 3. Visitors (`visitors.csv`)
| Column   | Description                                      |
|----------|--------------------------------------------------|
| date     | Date of user visit                               |
| group    | A/B test group (A or B)                          |
| visitors | Number of users in each group on that date       |

## 📈 Key Insights

- Compared ICE and RICE prioritization and evaluated shifts in hypothesis ranking.
- Visualized A/B test metrics (revenue, conversion rate, AOV) over time.
- Identified outliers based on 95th and 99th percentiles of user activity and revenue.
- Assessed statistical significance using non-parametric tests (Mann–Whitney U).
- Recommended actions based on test results.

## 🛠️ Tools & Technologies

- Python (Pandas, NumPy, SciPy, Matplotlib, Seaborn)
- Jupyter Notebook
- Statistical analysis and data visualization

## ✅ Final Decision

[Include here your conclusion: whether the test showed meaningful results and if any of the groups significantly outperformed the other.]

---

> Educational project from the [Yandex.Practicum](https://practicum.yandex.ru) Data Analyst course.
