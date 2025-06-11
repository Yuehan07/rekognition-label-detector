# AWS Rekognition Label Detection

This is a Python demo using **Amazon Rekognition** to detect labels from an image stored in S3 and visualize the results.

## 📷 Example Output

This image was analyzed using Amazon Rekognition. It detects multiple objects including people, cars, wheels, and clothing.

![Rekognition Output](https://github.com/Yuehan07/rekognition-label-detector/raw/main/rekognition_output.png)

## 🧰 AWS Services Used

- **Amazon Rekognition** – For label detection (bounding boxes, confidence scores)
- **Amazon S3** – Stores the image input
- **IAM** – Authenticates Python SDK access using boto3

## 🚀 How to Run

```bash
pip install -r requirements.txt
python test.py
