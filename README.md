## 🏥 Claim Error Detector
# Mini AI-Like Excel Project

**An AI-inspired, rule-based insurance claim validation system built entirely using Microsoft Excel.** 

# 📌 Project Overview

The Claim Error Detector is a lightweight, AI-inspired Excel system designed to automatically detect errors in insurance claims using logical rules, validations, and dashboard analytics.

This project simulates a real-world insurance workflow where:

-Claim data is entered

-Validations are applied automatically

-Claims are approved or rejected

-Insights are visualized through an interactive dashboard

# 🔍 Goal:
To demonstrate how Excel can mimic AI-style decision-making using rule-based logic and feature engineering — without VBA or coding.

# 🎯 Objectives

-Automate insurance claim validation

-Detect claim errors using rule-based logic

-Reduce manual verification effort

-Provide visual insights via dashboards

-Simulate AI-style classification using Excel

# 🧠 Key Features

✅ Structured claim data entry

🧮 Rule-based error detection engine

📄 Missing document validation

🛡 Policy status verification

🤖 Automated claim approval / rejection

📊 Dynamic dashboard with charts

🎨 Conditional formatting for instant alerts

🧱 Data Structure

## Sheet Name:Insurance_Claim_Data

| Column | Field Name            | Description                                         |
| ------ | --------------------- | --------------------------------------------------- |
| A      | `Claim_ID`            | Unique claim identifier                             |
| B      | `Policy_ID`           | Insurance policy number                             |
| C      | `Claim_Amount`        | Amount requested by claimant                        |
| D      | `Policy_Limit`        | Maximum allowed claim amount                        |
| E      | `Documents_Submitted` | Indicates if documents are submitted (`Yes` / `No`) |
| F      | `Policy_Status`       | Current policy state (`Active` / `Expired`)         |
| G      | `Amount_Valid`        | Auto-generated claim amount validation              |
| H      | `Doc_Valid`           | Document submission validation result               |
| I      | `Policy_Valid`        | Policy status validation result                     |
| J      | `Final_Status`        | Final claim decision (`Approved` / `Rejected`)      |



✔ Ensures the claim amount does not exceed the policy limit

2️⃣ Document Validation
=IF(E2="Yes","Valid","Invalid")


✔ Checks whether mandatory documents are submitted

3️⃣ Policy Status Validation
=IF(F2="Active","Valid","Invalid")


✔ Verifies that the policy is currently active

4️⃣ Final Claim Decision (Prediction Engine)
=IF(OR(G2="Invalid",H2="Invalid",I2="Invalid"),"Rejected","Approved")

📌 Prediction Logic

❌ If any validation fails → Rejected

✅ If all validations pass → Approved

This functions as a rule-based classification system, similar to decision engines used in real insurance platforms.

🎨 Conditional Formatting
Condition	Visual Indicator
Invalid values	🔴 Light Red

Approved claims	🟢 Light Green

Rejected claims	🔴 Red

✔ Enables quick visual identification of errors and claim outcomes.

📊 Dashboard Overview

Sheet Name: Dashboard

🔹 KPI Metrics

Total Claims

Approved Claims

Rejected Claims

🔹 Visual Charts
📈 Claim Status Distribution

Pie chart showing Approved vs Rejected claims

📊 Rejection Reasons

Column chart showing:

Amount Issue

Document Issue

Policy Issue

📌 All metrics and charts update dynamically as claim data changes.

📉 Business Insights

From the dashboard analysis:

📄 Missing documents are the leading cause of rejection

🛡 Policy issues are the second highest

💰 Amount limit violations occur less frequently

💡 Impact

These insights help insurers:

Improve document submission awareness

Reduce rejection rates

Optimize customer communication

🧠 Why This Project Is Unique

Uses Excel as an AI-like decision system

Applies feature engineering via validation columns

Simulates real insurance claim workflows

No VBA, macros, or external tools required

Beginner-friendly yet industry-relevant

🛠 Tools & Technologies Used

Microsoft Excel

Logical formulas

Conditional formatting

Charts & dashboards

Rule-based decision logic

📌 Use Cases

Insurance claim validation systems

Basic fraud detection modeling

Risk assessment training

Excel automation projects

Mini AI / analytics demonstrations

🚀 Future Enhancements

Add risk scoring mechanism

Introduce “Pending” claim status

Integrate slicers for filtering

Convert to Python / Flask backend

Implement ML-based prediction model
