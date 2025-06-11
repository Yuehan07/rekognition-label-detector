# 🧠 AWS Rekognition Label Detection Demo

This project demonstrates how to use **Amazon Rekognition** to automatically detect labels (such as Person, Car, Building, etc.) in an image stored in **Amazon S3**, and visualize the results using **Python** and **Matplotlib**.

It includes a full pipeline: upload → detect → visualize — with bounding boxes and confidence scores.

---

## 📊 Architecture Diagram

The following diagram illustrates how AWS services interact in this project:

![Architecture](https://github.com/Yuehan07/rekognition-label-detector/raw/main/e22ceb15-d5e2-437e-8a90-cefd8099162b.png)

---

## ☁️ AWS Services Used

| Service | Purpose |
|--------|---------|
| **Amazon Rekognition** | Detects labels in an image, returns objects, scenes, and bounding box coordinates |
| **Amazon S3** | Stores input images (e.g., `test.png`) |
| **IAM (Identity & Access Management)** | Authenticates access to AWS via credentials or CLI |
| **AWS CLI** | Provides access configuration for SDK (e.g., boto3 in Python) |

---

## 🚀 How to Run

### ✅ Prerequisites

- Python 3.10+
- AWS CLI configured with an IAM user that has:
  - `rekognition:DetectLabels`
  - `s3:GetObject`

### ✅ Installation

```bash
git clone https://github.com/Yuehan07/rekognition-label-detector.git
cd rekognition-label-detector
pip install -r requirements.txt
