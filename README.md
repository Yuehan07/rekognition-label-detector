# 🧠 AWS Rekognition Label Detection Demo

This project demonstrates how to use **Amazon Rekognition** to automatically detect labels (such as Person, Car, Building, etc.) in an image stored in **Amazon S3**, and visualize the results using **Python** and **Matplotlib**.

It includes a full pipeline: upload → detect → visualize — with bounding boxes and confidence scores.

---

## 📊 Architecture Diagram

The following diagram illustrates how AWS services interact in this project:

![Architecture](https://github.com/Yuehan07/rekognition-label-detector/raw/main/architecture.png)

---

## ☁️ AWS Services Used

| Service | Purpose |
|--------|---------|
| **Amazon Rekognition** | Detects labels in an image, returns objects, scenes, and bounding box coordinates |
| **Amazon S3** | Stores input images (e.g., `test.png`) |
| **IAM (Identity & Access Management)** | Authenticates access to AWS via credentials or CLI |
| **AWS CLI** | Provides access configuration for SDK (e.g., boto3 in Python) |

---

## 📷 Example Output

This image was analyzed using Amazon Rekognition. It detects multiple objects including people, cars, wheels, and clothing with bounding boxes and confidence scores:

![Rekognition Output](https://github.com/Yuehan07/rekognition-label-detector/raw/main/rekognition_output.png)

---

## 🏷️ Detected Labels (Top Results)

| Label     | Confidence (%) |
|-----------|----------------|
| Person    | 98.27          |
| Car       | 94.61          |
| Building  | 91.50          |
| Shoe      | 89.12          |
| Wheel     | 85.77          |
| Clothing  | 83.45          |
| Street    | 79.88          |

> *Note: Confidence scores and results may vary depending on the input image.*

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

### 🏷️ Detected Labels (Top Results)

| Label     | Confidence (%) |
|-----------|----------------|
| Person    | 98.27          |
| Car       | 94.61          |
| Building  | 91.50          |
| Shoe      | 89.12          |
| Wheel     | 85.77          |
| Clothing  | 83.45          |
| Street    | 79.88          |

> *Note: Confidence scores and results may vary depending on the input image.*

---

## 🧠 Learning Outcomes

- 🔧 How to use `boto3` to interact with Amazon Rekognition
- 📦 How to read images from S3 using Python
- 📊 How to display detected labels with bounding boxes using `matplotlib`
- 🔐 How to resolve IAM and S3 permission issues
- 🌏 How to ensure region alignment between S3 and Rekognition

---

## 🧑‍💻 Author

👋 Hi! I'm **Olivia**, an aspiring cloud and product enthusiast exploring AWS services through hands-on projects.

Feel free to ⭐ star or 🍴 fork the repository if you find it useful, or connect with me on [GitHub](https://github.com/Yuehan07)!
