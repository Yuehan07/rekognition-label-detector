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


## 🔍 Example Output

This image was analyzed using Amazon Rekognition. It detects multiple objects including people, cars, wheels, and clothing with high confidence:

![Rekognition Output](https://github.com/olivia-chen/rekognition-label-detector/raw/main/rekognition_output.png)

