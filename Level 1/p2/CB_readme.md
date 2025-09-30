# 💰 AWS Cost Budget Setup

This project demonstrates how I created an **AWS Cost Budget** to monitor and control my spending.  
It was one of my beginner-level tasks to understand **AWS Budgets** and practice cost management.

---

## 📌 Task Overview
- Created a **Cost Budget** with a limit of **$5**.  
- Configured alerts so I get notified when my usage approaches or exceeds the budget.  
- Helps me avoid unexpected AWS charges during practice and learning.

---

## 🛠️ Steps I Followed

1. **Opened AWS Budgets Console**  
   - Navigated to **Billing & Cost Management → Budgets**.

2. **Created a New Budget**  
   - Type: **Cost Budget**  
   - Period: **Monthly**  
   - Amount: **$5**

3. **Set Alerts**  
   - Configured thresholds for 80% and 100% of the budget.  
   - Connected to my **email** via Amazon SNS for notifications.

4. **Reviewed and Saved**  
   - Verified that the budget shows up in the Budgets dashboard.  
   - Tested notifications to confirm setup works.

---

### You need to answer the following:
## 1. In order for IAM users to create budgets in the Billing and Cost Management console what else must these users be allowed to do? <br/>
**Ans.** To allow IAM users to create budgets in the Billing and Cost Management console, they must have specific permissions to access the service. The required permissions include:

* **budgets:CreateBudget** – Allows the creation of budgets.
* **aws-portal:ViewBilling** – Enables viewing billing information.
* **budgets:ViewBudget** – Grants access to view and manage existing budgets.
These permissions are often found in policies such as **AWSBillingReadOnlyAccess** or **AWSBudgetsActionsPolicy**.

Additionally, the account owner needs to enable IAM User and Role Access to Billing Information for IAM users to access billing details. <br />

## 2. In addition to the console how else can you create budgets? <br />
**Ans.** In addition to using the AWS Billing and Cost Management Console, you can create budgets through the following methods:
1. **AWS Command Line Interface (CLI):**
    - You can use the AWS CLI to create budgets programmatically by executing commands like aws budgets create-budget. This method allows for automation and integration with scripts.
2. **AWS SDKs:**
    - You can create budgets using various AWS SDKs (e.g., Python, Java, Node.js, etc.). This is useful for developers who want to integrate budget creation into their applications or workflows.
3. **AWS CloudFormation:**
    - Budgets can be created via AWS CloudFormation templates. This is useful for setting up budgets as part of an infrastructure deployment.
4. **AWS Budgets API:**
    - You can interact directly with the AWS Budgets API to create, update, and manage budgets. This is typically used by developers or systems that require programmatic access to budget creation.

## 3. Is it better to set budgets on a recurring basis or for a specific time? And why?
**Ans.** Whether to set AWS budgets on a recurring basis or for a specific time depends on your use case and financial management needs. Here's a comparison of both approaches:

  * **Recurring budgets** are better for most users, especially for regular cloud operations or business applications, as they offer ongoing monitoring and control over long-term spending.
  
  * **Specific-time budgets** are useful for one-off projects, events, or time-bound workloads where you want to monitor and limit costs within a specific time frame.

 ## 4. What are the different types of costs that make up a cost budget? <br />
**Ans.** A cost budget in AWS typically consists of several different types of costs that can be tracked and managed. These cost components include:
1. **Service Costs:** Charges for using AWS services (e.g., EC2, S3).
2. **Reserved Instance or Savings Plans Costs:** Discounts for long-term commitments.
3. **Data Transfer Costs:** Charges for moving data between services or regions.
4. **Support Plan Costs:** Fees for AWS support plans.
5. **Third-Party Costs:** Purchases from the AWS Marketplace.
6. **Taxes and Fees:** Applicable taxes, like VAT or sales tax.
7. **Cost Allocation Tags:** Categorized spending by project or department.
8. **Usage Costs:** Pay-as-you-go charges based on resource consumption. <br />

## 5. What are the different options for setting budget alerts? <br />
**Ans.** AWS provides several options for setting budget alerts, allowing you to track and manage your spending effectively. These options include:
1. **Cost Budget Alerts** - Notify when actual or forecasted costs exceed a set limit.
2. **Usage Budget Alerts** - Alert when service usage surpasses thresholds.
3. **Reservation Budget Alerts** - Track reserved instance or savings plan usage.
4. **Forecasted Alerts** - Warns before reaching future budget limits.
5. **Percentage-Based Alerts** - Trigger alerts at specific budget percentages (e.g., 50%, 80%).
6. **Custom Timeframe Alerts** - Set for monthly, quarterly, or annual budgets
<br />

![Cost Budget image](https://github.com/tejas-firke/Portfolio-projects/blob/0e0bfab0cda33f74fd3626de07baa826f2d9b768/New%20folder/Level%201/p2/Screenshot%202025-09-25%20142915.png)
