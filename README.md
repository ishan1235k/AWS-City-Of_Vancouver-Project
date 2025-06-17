# City of Vancouver Employee Data Quality Control

This project implements a data quality control pipeline for the City of Vancouver’s Employee Remuneration and Expenses dataset using AWS Glue Studio. The pipeline ensures data accuracy by applying completeness, uniqueness, and value validation rules. It also ensures data security through encryption, versioning, replication, and enables governance through monitoring and auditing.

---

## AWS KMS Key Management
To secure the data at rest, I created three customer-managed keys in AWS KMS: `RawBucketKeyCoVIshan`, `CleanBucketKeyCoVIshan`, and `CuratedBucketKeyCoVIshan`. Each key protects its respective S3 bucket for fine-grained control and auditing.
![KMS Keys](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-14%20134529.png)

---

## S3 Bucket Encryption (Raw Bucket)
Enabled server-side encryption using SSE-KMS on the raw bucket with its KMS key.
![S3 Encryption Raw](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-14%20134740.png)

---

## S3 Bucket Versioning (Raw Bucket)
Enabled versioning on the raw bucket to preserve object history and recover from accidental deletions.
![S3 Versioning Raw](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-14%20134841.png)

---

## S3 Bucket Encryption (Clean Bucket)
Enabled SSE-KMS encryption on the clean bucket with its designated KMS key.
![S3 Encryption Clean](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-14%20135553.png)

---

## S3 Bucket Versioning (Clean Bucket)
Enabled versioning on the clean bucket for data recovery and audit history.
![S3 Versioning Clean](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-14%20135448.png)

---

## S3 Replication (Clean Bucket)
Set up replication from clean bucket to another bucket in the same region for durability and disaster recovery.
![S3 Replication Clean](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-14%20141042.png)

---

## S3 Bucket Encryption (Curated Bucket)
Enabled SSE-KMS encryption on the curated bucket.
![S3 Encryption Curated](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-14%20140412.png)

---

## S3 Bucket Versioning (Curated Bucket)
Versioning ensures all curated data versions are preserved.
![S3 Versioning Curated](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-14%20140327.png)

---

## AWS Glue Job Flow
Created an ETL job in Glue Studio named `emp-Cov-Ishan-QC` that loads raw data, applies quality checks, and routes data.
![Glue Job Flow](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-14%20235608.png)

---

## Data Quality Rules
Defined completeness, uniqueness, and valid value range rules in the Glue Data Quality transform.
![Data Quality Rules](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-14%20235635.png)

---

## Route Transform Results
Configured routing to send passed records to curated data and failed records to rejected data S3 location.
![Route Transform](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-15%20000758.png)

---

## CloudWatch Dashboard
Built a CloudWatch dashboard to monitor S3 storage, Glue, KMS, Athena costs, and other AWS resource usage.
![CloudWatch Dashboard](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-15%20130928.png)



## CloudTrail Logs
Enabled CloudTrail to log all management events for auditing and compliance.
![CloudTrail Logs](https://github.com/ishan1235k/Screenshots/blob/main/Screenshot%202025-06-15%20134209.png)

---

## How to Run
1. Upload data to raw S3 bucket.
2. Run the Glue job.
3. Review curated and rejected data in S3.
4. Use CloudWatch and CloudTrail to monitor and audit.

---

