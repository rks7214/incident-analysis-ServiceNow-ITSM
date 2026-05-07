# incident-analysis-ServiceNow-ITSM 
# Incident Analysis & Automated Email Notification (ServiceNow)

## 📌 Overview
When multiple incidents are created for the same issue, a problem should be created to address the root cause. However, manually identifying repeated incidents is time-consuming and inefficient.
To solve this, I developed an automated solution using ServiceNow Flow Designer that identifies recurring incidents based on specific conditions and sends notifications to authorized users for problem creation.

## 🎯 Objective
- Reduce manual effort in identifying repeated incidents
- Improve ITSM efficiency using automation
- Support proactive problem management

## 🛠️ Tools & Technologies
- ServiceNow
- Flow Designer

## ⚙️ Solution Design
The solution uses Flow Designer to:
1. Trigger when a new incident is created
2. Check for similar incidents within the last 7 days
3. Count incidents with the same configuration item
4. If count ≥ 3, send notification email to assigned group

## 🚀 Key Features
- Automated incident analysis
- Threshold-based condition (≥ 3 incidents)
- Role-based email notification
- Reduces manual monitoring effort

## 🧪 Testing
- Created multiple incidents with same configuration item
- Verified flow trigger execution
- Checked email notification via inbound email logs

