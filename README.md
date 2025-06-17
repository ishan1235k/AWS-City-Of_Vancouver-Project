# DataQualityControl in AWS
# City of Vancouver Employee Data Quality Control

This project implements a data quality control pipeline for the City of Vancouver’s Employee Remuneration and Expenses dataset using AWS Glue Studio. The pipeline ensures data accuracy by applying completeness, uniqueness, and value validation rules, and separates clean and rejected data automatically.

---

## Project Objective
Ensure only high-quality data is used for analytics. Automate data cleaning using AWS Glue Studio. Secure data with encryption, versioning, and replication. Provide monitoring through AWS CloudWatch and auditing through AWS CloudTrail.

---

## AWS Glue Job Flow
![AWS Glue Job Flow](Screenshot 2025-06-14 134529.png)

---

## Data Quality Rules
![Data Quality Rules](https://raw.githubusercontent.com/ishan1235k/Screenshots/main/your-data-quality-rules-image.png)

---

## Route Transform Results
![Route Transform Results](https://raw.githubusercontent.com/ishan1235k/Screenshots/main/your-route-transform-image.png)

---

## S3 Bucket Encryption
![S3 Bucket Encryption](https://raw.githubusercontent.com/ishan1235k/Screenshots/main/your-s3-encryption-image.png)

---

## S3 Versioning
![S3 Versioning](https://raw.githubusercontent.com/ishan1235k/Screenshots/main/your-s3-versioning-image.png)

---

## S3 Replication
![S3 Replication](https://raw.githubusercontent.com/ishan1235k/Screenshots/main/your-s3-replication-image.png)

---

## CloudWatch Dashboard
![CloudWatch Dashboard](https://raw.githubusercontent.com/ishan1235k/Screenshots/main/your-cloudwatch-dashboard-image.png)

---

## Billing Alarm
![Billing Alarm](https://raw.githubusercontent.com/ishan1235k/Screenshots/main/your-billing-alarm-image.png)

---

## CloudTrail Events
![CloudTrail Events](https://raw.githubusercontent.com/ishan1235k/Screenshots/main/your-cloudtrail-events-image.png)

---

## How to Run
1. Upload the data to the raw S3 bucket.
2. Run the AWS Glue job from Glue Studio.
3. Check S3 for cleaned and rejected data outputs.
4. Use Athena or another tool to analyze the curated data.
5. Monitor costs and usage through CloudWatch.

---

## Notes
- Screenshots are loaded from: [Screenshots Repo](https://github.com/ishan1235k/Screenshots)
- Ensure that file names in the links above exactly match your uploaded files.
