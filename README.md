# AWS Rekognition Label Detection

A simple demo that uses **Amazon Rekognition** to detect labels in an image stored in S3, and visualizes bounding boxes using Python.

## 🧰 AWS Services Used

- **Amazon Rekognition** – Detect labels in an image (e.g., Person, Street, Car)
- **Amazon S3** – Host the input image (test.png)
- **IAM** – Control access to AWS services via user credentials

## 📦 Python Dependencies

- `boto3`
- `matplotlib`
- `pillow`

## 💻 How to Run

```bash
pip install -r requirements.txt
python test.py

![image](https://github.com/user-attachments/assets/56fc049e-94c9-4230-9f39-83028e33e888)
