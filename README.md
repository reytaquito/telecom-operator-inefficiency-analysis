# Telecom Operator Inefficiency Analysis

## 📄 Project Description

CallMeMaybe, a virtual telephony service, needs to identify its least effective operators. An operator is deemed **inefficient** if they exhibit:

- A high number of missed incoming calls (both internal and external).  
- Long average wait times for incoming calls.  
- (If applicable) A low volume of outgoing calls.

This repository provides:

1. **Exploratory Data Analysis** of call logs to surface usage patterns.  
2. **Identification** of inefficient operators based on key metrics.  
3. **Statistical Testing** (hypothesis tests) to confirm whether observed inefficiencies are significant.

---

## 🗂️ Data Description

The datasets include:

- **incoming_calls.csv**: Records of all incoming calls (timestamp, operator_id, status, wait_time).  
- **outgoing_calls.csv**: Records of outgoing calls (timestamp, operator_id, duration).  
- **internal_calls.csv**: Records of internal calls between operators (timestamp, from_operator_id, to_operator_id, duration).  
- **operators.csv**: Operator metadata (operator_id, team, shift, role).

---

## 🎯 Objectives

1. **Explore** call volume, drop rates, and wait times per operator.  
2. **Compute** performance metrics:
   - Missed incoming call rate  
   - Average wait time  
   - Outgoing call count  
3. **Rank** operators by inefficiency and flag those below performance thresholds.  
4. **Perform** statistical tests (e.g., chi‑square, t‑tests) to validate whether inefficiency differences are statistically significant.

---
