# AI-Powered Model Training and Deployment Pipeline

Welcome to our AI Model Pipeline. This project showcases the complete lifecycle of building, training, evaluating, and deploying a machine learning model using a modern MLOps workflow.

<p align="center">
  <img src="https://img.shields.io/badge/Status-Deployed-brightgreen?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Model-Trained-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/MLOps-Pipeline-blueviolet?style=for-the-badge"/>
</p>

---

## Overview

This project addresses the real-world challenge of manually verifying and assigning applicants to the correct sub-schemes under the **National Social Assistance Program (NSAP)**—a critical welfare initiative by the Government of India.

The system uses machine learning to **predict the correct NSAP scheme** for each applicant, reducing human error and accelerating aid distribution.

Key highlights:
- End-to-end machine learning pipeline design
- Automated data processing, model training, and evaluation
- Leaderboard-based model selection
- Seamless deployment for real-time or batch inference

The pipeline is built to be scalable, modular, and easily adaptable to other government schemes or datasets.

---

## Data Collection

- **Source**: AI Kosh NSAP dataset
- **Features**: Age, gender, income level, disability status, marital status
- **Labels**: Scheme codes
  - IGNOAPS (Old Age)
  - IGNWPS (Widow)
  - IGNDPS (Disability)

---

## Data Preprocessing

- Removed or handled missing/inconsistent values
- Categorical fields encoded into numerical format
- Data normalized where required
- Balanced dataset using under/over sampling techniques

---

## Machine Learning Model

- **Model Used**: Random Forest Classifier
- **Platform**: IBM Watsonx.ai
- **Task**: Multi-class classification
- **Goal**: Predict the most suitable NSAP sub-scheme based on applicant details

---

## Training Pipeline

The training pipeline is fully automated and includes the following stages:
- Data preprocessing
- Model training
- Model evaluation and validation
- Leaderboard generation for ranking models

### Training Process Snapshots

| Step                     | Screenshot |
|--------------------------|------------|
| Training Initialization  | ![Training 1](https://github.com/user-attachments/assets/1f230b39-73a8-4ce7-a38e-3e49161ba2c5) |
| Evaluation Started       | ![Training 2](https://github.com/user-attachments/assets/9d37a109-c2cf-49cb-b82b-25538d8a6877) |

---

## Leaderboard

After training, all models are evaluated and ranked based on defined metrics (accuracy, F1-score, etc.). The leaderboard helps in selecting the top-performing model for deployment.

![Leaderboard](https://github.com/user-attachments/assets/d9c72608-ceee-48e6-986e-c75319ccfcd6)

---

## Deployment

The top-performing model is deployed online via Watsonx.ai for real-time predictions on new applicant data.

![Deployed](https://github.com/user-attachments/assets/4a3273ee-165e-4db5-8c43-380baf44479e)

---

## Result after Testing

The deployed model was tested to ensure real-world readiness. The system outputs confidence scores with each prediction, aiding human decision-makers.

Example results:
- IGNDPS – 70%
- IGNOAPS – 60%
- IGNWPS – 70%

![Test Result](https://github.com/user-attachments/assets/9d572280-ea9e-414c-9875-29202792d83b)

---

## Evaluation

- Accuracy: Verified through test set performance
- Confidence scores: Range from 50% to 70%
- Faster processing: Significantly reduces manual verification time
- Transparent results: Confidence scores enable better decision-making

---

## Tech Stack

- Python
- IBM Watsonx.ai
- GitHub Actions
- MLOps pipeline orchestration tools

---

## Key Features

- Fully automated and reproducible ML pipeline
- Model evaluation and ranking with leaderboard
- Fast, real-time deployment on IBM Watsonx.ai
- Accurate predictions with confidence scores
- Designed for scalability and reusability in other government schemes

---

> Built with precision. Deployed with purpose.
