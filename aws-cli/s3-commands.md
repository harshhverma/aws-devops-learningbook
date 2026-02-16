# AWS CLI - S3 Commands

This document contains practical S3 operations performed using AWS CLI.

## 1. List All Buckets

aws s3 ls

## 2. Create a Bucket (us-east-1)

aws s3api create-bucket \
  --bucket harsh-devops-lab-bucket \
  --region us-east-1

## Notes:
Bucket names must be globally unique.
No uppercase letters allowed.
us-east-1 does not require LocationConstraint.

## 3. Create a Bucket in Another Region (Example: ap-south-1)

aws s3api create-bucket \
  --bucket harsh-devops-lab-bucket \
  --region ap-south-1 \
  --create-bucket-configuration LocationConstraint=ap-south-1
## Required when creating bucket outside us-east-1.


## 4. Upload File to Bucket

aws s3 cp file.txt s3://harsh-devops-lab-bucket/

Uploads a file to the specified S3 bucket.


## 5. List Objects Inside a Bucket

aws s3 ls s3://harsh-devops-lab-bucket

Displays all objects stored in the bucket.


## 6. Download File from Bucket

aws s3 cp s3://harsh-devops-lab-bucket/file.txt .

Downloads the file to the current directory.


## 7. Delete a File from Bucket

aws s3 rm s3://harsh-devops-lab-bucket/file.txt
Deletes a specific object from the bucket.


## 8. Remove an Empty Bucket

aws s3 rb s3://harsh-devops-lab-bucket
The bucket must be empty before deletion.


## 9. Remove Bucket with All Objects (Force Delete)

aws s3 rb s3://harsh-devops-lab-bucket --force
Deletes the bucket along with all objects inside it.


## Important Points
Bucket names are globally unique across AWS.
Always verify region before creating a bucket.
Avoid making buckets public unless necessary.
Clean up unused buckets to avoid unexpected storage charges.
