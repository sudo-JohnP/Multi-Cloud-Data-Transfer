# 🌐 Multi-Cloud Data Transfer with AWS and GCP

This project demonstrates how to securely transfer data between **AWS S3** and **Google Cloud Storage (GCS)** using identity federation and GCP’s **Storage Transfer Service**. It was completed as part of a hands-on cloud challenge on [NextWork](https://learn.nextwork.org/).

## 🚀 Objective

Showcase the ability to:
- Set up and configure cloud storage services in **AWS** and **GCP**
- Securely connect two different cloud providers using **IAM roles** and **identity federation**
- Perform a **batch data transfer** between S3 and GCS

---

## 🧰 Tools & Services Used

| AWS                        | GCP                                  |
|---------------------------|--------------------------------------|
| S3 (Source Bucket)         | Cloud Storage (Destination Bucket)   |
| IAM (Trust Policy Setup)   | Storage Transfer Service             |
| Identity Federation        | GCP IAM Roles                        |

---

## 📦 Project Steps

**Diagram Overview**
- <img width="867" height="615" alt="Multi_Cloud_Data_Transfer_Graphic" src="https://github.com/user-attachments/assets/b8ef887b-ff2c-4b77-9309-aa74398e0760" />


### 1. Set Up AWS S3 Bucket
- Created and uploaded sample files to an S3 bucket to serve as source data.
- <img width="1866" height="716" alt="File_Upload_S3" src="https://github.com/user-attachments/assets/6a24ed66-32e9-4dd8-b44b-3941f0b17a09" />


### 2. Set Up Google Cloud Platform
- Initialized a GCP project using free-tier credits.
- Created a GCP bucket with appropriate region and storage class settings.
- <img width="1512" height="828" alt="GCP_Backup_Bucket" src="https://github.com/user-attachments/assets/3a88652c-29fc-419e-9964-96aae42f879c" />


### 3. IAM Identity Federation
- Created a custom **IAM role** in AWS with a trust policy for GCP access.
- Granted GCP temporary read access to the S3 bucket using a **subject ID**.
- <img width="1872" height="806" alt="AWS_Trust_Policy" src="https://github.com/user-attachments/assets/89a5a73a-4034-4831-8062-81d6297130f1" />


### 4. Configure Storage Transfer
- Used **GCP's Storage Transfer Service** to create a **batch job**.
- Verified success by checking for transferred files in the GCP bucket.
- <img width="707" height="765" alt="GCP_Transfer_Setup" src="https://github.com/user-attachments/assets/11cd9ed9-bee7-4aa1-9330-1bf88ea59ee7" />

---

## ✅ Results

✔️ Successfully transferred files from AWS to GCP  
✔️ Used IAM roles and identity federation for secure, temporary access  
✔️ Demonstrated understanding of **multi-cloud interoperability**

---

## 💬 Reflection

This project took about an hour to complete. The biggest challenge was navigating the **GCP interface** for the first time, but it was rewarding to see a successful transfer between two major cloud platforms. I now feel more confident working in **multi-cloud environments** and understanding **cloud identity and access management (IAM)** across providers.

---

## 📚 Skills Demonstrated

- Multi-Cloud Infrastructure
- AWS S3 & IAM
- Google Cloud Storage
- Identity Federation
- Cloud Data Transfer Workflows
- Security Best Practices for Cloud Access

---

## 🔗 NextWork

This project was completed via the [NextWork](https://learn.nextwork.org/) platform — a resource for building and showcasing real-world technical projects.

