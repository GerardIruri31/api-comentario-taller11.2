# Comment API – AWS Lambda, DynamoDB, S3 & Linux Automation

This project exposes a simple HTTP API to create comments.  
Each request is processed by an AWS Lambda function that:

1. Stores the comment in **DynamoDB**.
2. Pushes the same record as a JSON file to **S3** (push ingestion pattern).
3. Returns the inserted item and S3 location in the response.

A Linux shell script (`verify_comentario.sh`) automates end-to-end tests across **dev**, **test** and **prod** stages.

---
