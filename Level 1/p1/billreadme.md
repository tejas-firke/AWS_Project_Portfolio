# 💰 AWS Billing Alarm Setup

This project demonstrates how I created **AWS CloudWatch Billing Alarms** to monitor my account usage and receive alerts when costs cross specific thresholds.  
It was one of my beginner-level tasks to get hands-on with **AWS Billing & CloudWatch**.

---

## 📌 Task Overview

- Created **billing alarms** for my AWS account at:
  - **$1**
  - **$5**
  - **$10**
- These alarms help me track and control costs by sending notifications when the threshold is reached.

---

## 🛠️ Steps I Followed

1. **Enabled Billing Alerts**  
   - Went to **Billing & Cost Management Console** → **Billing Preferences**  
   - Enabled `Receive Billing Alerts`.

2. **Created SNS Topic (Notification Service)**  
   - Created an **SNS Topic** to send email notifications.  
   - Subscribed my email to the topic and confirmed it.

3. **Created CloudWatch Billing Alarms**  
   - Opened **CloudWatch Console** → **Alarms** → **Create Alarm**.  
   - Chose **Billing Metric** → `Total Estimated Charge`.  
   - Set thresholds for **$1, $5, and $10**.  
   - Linked the alarms to my **SNS Topic**.

4. **Tested Notifications**  
   - Verified that emails are received when the threshold is crossed.

---

###  You need to answer the following: 

## 1. How many billing alarms do you get for free?

We can create up to 10 billing alarms for free as part of the AWS Free Tier.

## 2. When a billing alarm is triggered how will you know?

When a billing alarm is triggered, we will receive a notification via Amazon Simple Notification Service (SNS). This can be configured to send alerts through email, SMS, or other endpoints.

## 3. What is the difference between a billing alarm and a cloudwatch alarm?

* **Billing Alarm:** Specifically monitors your AWS account’s estimated charges. It triggers when your charges exceed a specified threshold. Billing alarms are based on billing data and are used to help manage and control costs.

* **CloudWatch Alarm:** Monitors a variety of metrics related to AWS resources and applications, such as CPU usage, memory usage, and custom metrics. These alarms can trigger actions like sending notifications or automatically scaling resources based on the defined thresholds

![Billing alarm ss](https://github.com/tejas-firke/Portfolio-projects/blob/476194e5b1c829b0759651e7cae05c1a1485d5ba/New%20folder/Level%201/p1/Screenshot%202025-09-29%20130116.png)
