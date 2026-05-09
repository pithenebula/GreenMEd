# GreenMed - Medicine Recommendation System

GreenMed is a Machine Learning based healthcare web application that predicts diseases from user-provided symptoms and provides personalized recommendations including medications, precautions, diet plans, and workout suggestions.

The project combines Machine Learning, Data Processing, and Web Development to create an intelligent healthcare assistance system using Python and Flask.

---

# Project Overview

The main objective of this project is to develop a smart healthcare recommendation system capable of predicting diseases based on symptoms entered by users.

After predicting the disease, the system provides:
- Disease description
- Recommended medications
- Precautionary measures
- Diet suggestions
- Workout recommendations

The system is designed as a real-time web application using Flask and a Support Vector Classifier (SVC) Machine Learning model.

---

# Features

- Disease prediction using Machine Learning
- Symptom-based diagnosis system
- Real-time prediction
- Medicine recommendation
- Precaution suggestion
- Diet recommendation
- Workout recommendation
- User-friendly web interface
- Flask-based backend integration

---

# Technologies Used

## Programming Language
- Python

## Frontend
- HTML
- CSS
- Bootstrap

## Backend
- Flask

## Machine Learning
- Scikit-learn
- Support Vector Classifier (SVC)

## Libraries
- NumPy
- Pandas
- Pickle

---

# Machine Learning Model

This project uses a pre-trained Support Vector Classifier (SVC) model for disease prediction.

The model predicts diseases based on symptoms entered by the user.

## Workflow

1. User enters symptoms
2. Symptoms are cleaned and processed
3. Symptoms are converted into a binary feature vector
4. The SVC model predicts the disease
5. Additional information is retrieved from datasets
6. Results are displayed on the web page

---

# Dataset Information

The system uses multiple CSV datasets containing healthcare-related information.

| Dataset | Purpose |
|---|---|
| symptoms_df.csv | Symptoms dataset |
| precautions_df.csv | Precaution suggestions |
| description.csv | Disease descriptions |
| medications.csv | Medicine recommendations |
| diets.csv | Diet plans |
| workout_df.csv | Workout suggestions |

---

# Project Structure

```bash
GreenMed/
│
├── app.py
│
├── datasets/
│   ├── symtoms_df.csv
│   ├── precautions_df.csv
│   ├── workout_df.csv
│   ├── description.csv
│   ├── medications.csv
│   └── diets.csv
│
├── models/
│   └── svc.pkl
│
├── templates/
│   ├── index.html
│   ├── about.html
│   ├── contact.html
│   ├── developer.html
│   └── blog.html
│
├── static/
│
├── requirements.txt
│
└── README.md
```

---

# System Architecture

```text
User Input Symptoms
        ↓
Flask Backend
        ↓
Symptom Preprocessing
        ↓
Binary Feature Vector Creation
        ↓
SVC Machine Learning Model
        ↓
Disease Prediction
        ↓
Recommendation Retrieval
        ↓
Display Result to User
```

---

# Installation Guide

## Step 1: Clone the Repository

```bash
git clone https://github.com/pithenebula/GreenMed.git
cd GreenMed
```

---

## Step 2: Create Virtual Environment

```bash
python -m venv venv
```

---

## Step 3: Activate Virtual Environment

### Windows

```bash
venv\Scripts\activate
```

### Linux/Mac

```bash
source venv/bin/activate
```

---

## Step 4: Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Required Libraries

```bash
Flask
numpy
pandas
scikit-learn
pickle-mixin
```

---

# Run the Project

```bash
python app.py
```

After running the project, open your browser and visit:

```bash
http://127.0.0.1:5000/
```

---

# Example Input

```text
itching, skin rash, fatigue
```

---

# Example Output

```text
Predicted Disease: Fungal Infection

Description:
Fungal infection is a skin disease caused by fungi.

Precautions:
- Keep skin clean
- Avoid sweating
- Use clean clothes
- Maintain hygiene

Medications:
- Antifungal cream
- Antifungal tablets

Diet:
- Protein-rich foods
- Vitamin-rich foods

Workout:
- Light exercise
```

---

# Screenshots

## Home Page
<img src="blob:https://web.whatsapp.com/e445d301-c609-4d4d-8b90-98dfffb40fc5"/><img width="1001" height="524" alt="image" src="https://github.com/user-attachments/assets/cb2be339-7d52-4f8c-9f15-8dc827c2489d" />


---

## Symptom Input
<img src="blob:https://web.whatsapp.com/66be7fa9-1f6c-4cad-aac4-ffe627fc5c78"/><img width="953" height="501" alt="image" src="https://github.com/user-attachments/assets/1d86287b-cf38-4ff9-9fee-74841d10db3a" />


---

## Prediction Output
<img src="blob:https://web.whatsapp.com/6382941e-64a3-4b7d-b962-d8c52cc9f61b"/><img width="868" height="587" alt="image" src="https://github.com/user-attachments/assets/c060827a-b3b5-4bc4-a09b-1dd621af581c" />


---

# Key Functionalities

## Symptom Preprocessing

The system converts user-entered symptoms into machine-readable format by:
- converting text to lowercase
- replacing spaces with underscores
- mapping symptoms to numerical indices

---

## Binary Feature Vector

The model uses a binary vector where:

- `1` = symptom present
- `0` = symptom absent

Example:

```text
[1,0,1,0,0,1...]
```

---

## Disease Prediction

The processed feature vector is passed to the SVC model which predicts the disease.

---

## Recommendation System

After prediction, the system retrieves:
- disease description
- medications
- precautions
- diet plans
- workouts

from multiple datasets.

---

# Advantages

- Fast disease prediction
- User-friendly interface
- Real-time recommendations
- Educational healthcare application
- Demonstrates practical ML integration

---

# Limitations

- Limited number of diseases
- Depends on dataset quality
- Cannot replace professional doctors
- Limited symptom coverage

---

# Future Improvements

- Add Deep Learning models
- Increase dataset size
- Improve prediction accuracy
- Mobile application development
- Doctor consultation feature
- User authentication system
- Cloud deployment





---

# License

This project is developed for educational and academic purposes only.

---

# Acknowledgements

- Flask Documentation
- Scikit-learn Documentation
- Pandas Documentation
- NumPy Documentation
- Healthcare datasets used for research and development

---

# Conclusion

GreenMed demonstrates how Machine Learning can be integrated with web technologies to create intelligent healthcare applications. The system successfully predicts diseases from symptoms and provides personalized healthcare recommendations through a simple and interactive web interface.
