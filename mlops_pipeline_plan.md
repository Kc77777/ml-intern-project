# 🧪 MLOps Pipeline Plan – Aavas Kc

## 1. Where will you store your data and model?
I will store the dataset and the trained model in the cloud — for example, on Google Cloud Storage or AWS S3. This ensures it’s accessible for training, inference, and retraining from any environment.

## 2. How will you retrain the model later if new data comes?
I'll pull the latest data from the source (like a cloud database or API), and then retrain the model using a script. This can be automated with a scheduled job (e.g., cron or CI/CD pipeline).

## 3. How do you know if the model gets worse?
I’ll track performance metrics (like accuracy). If the accuracy drops below 90%, that will be my signal to investigate or retrain the model.

## 4. How do you expose the model to other apps or users?
I’ll package the model into a REST API using FastAPI or Flask, and then integrate that API into the target app (web, mobile, or dashboard) so it can provide live predictions.
