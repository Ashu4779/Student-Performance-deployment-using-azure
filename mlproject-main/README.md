Student Performance Predictor
This project is an end-to-end machine learning application designed to predict student performance based on a number of key indicators. It features a complete ML pipeline for data processing and model training, and a user-friendly web interface for real-world interaction. The application is deployed on Azure.

🚀 Features
End-to-End ML Pipeline: Implements a full pipeline including data ingestion, feature engineering, data transformation, and model training.

Web Interface: A clean and simple UI built with Flask to allow users to input student data and receive performance predictions.

Modular Code: The project is structured with modular components for easy maintenance and scalability.

Cloud Deployment: Ready for production and deployed on Microsoft Azure.

Data Exploration: Includes Jupyter notebooks for exploratory data analysis (EDA) and model experimentation.

🛠️ Tech Stack
Backend: Python, Flask

ML/Data Science: Scikit-learn, Pandas, NumPy, Seaborn, Matplotlib

Deployment: Microsoft Azure, Docker (optional for local containerization)

Frontend: HTML, CSS

📂 Project Structure
The repository is organized as follows:

.
├── .github/                    # Contains CI/CD workflows
├── notebook/                   # Jupyter notebooks for EDA and model building
│   ├── 1. EDA.ipynb
│   └── 2. Model.ipynb
├── src/                        # Source code for the ML application
│   ├── components/             # Core ML pipeline components
│   │   ├── __init__.py
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   ├── pipeline/               # Manages the execution of the ML pipelines
│   │   ├── __init__.py
│   │   ├── predict_pipeline.py
│   │   └── train_pipeline.py
│   ├── __init__.py
│   ├── exception.py            # Custom exception handling
│   ├── logger.py               # Logging configuration
│   └── utils.py                # Utility functions
├── static/                     # CSS files for styling
├── templates/                  # HTML templates for the web app
│   ├── home.html
│   └── index.html
├── application.py              # Main Flask application entry point
├── requirements.txt            # Project dependencies
├── setup.py                    # Setup script for making the project a package
└── README.md

⚙️ Setup and Installation
To run this project locally, please follow these steps:

1. Clone the Repository:

git clone https://github.com/Ashu4779/Student-Performance-deployment-using-azure.git
cd Student-Performance-deployment-using-azure/mlproject-main

2. Create a Virtual Environment:
It's highly recommended to use a virtual environment to manage dependencies.

Using conda:

conda create -p venv python==3.8 -y
conda activate venv/

Using venv:

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

3. Install Dependencies:
Install all the required packages from the requirements.txt file.

pip install -r requirements.txt

▶️ How to Run
1. Run the Flask Application:
Execute the main application file to start the web server.

python application.py

2. Access the Application:
Open your web browser and navigate to the following address:

http://127.0.0.1:5000

3. Make a Prediction:
On the home page, fill in the form with the student's details and click "Predict" to see the predicted performance score.

☁️ Deployment on Azure
This application is deployed on Microsoft Azure, providing a scalable and reliable environment for the prediction service. The deployment process typically involves:

Containerizing the application using Docker.

Pushing the Docker image to a container registry (like Azure Container Registry).

Deploying the image to an Azure App Service or Azure Kubernetes Service (AKS).

👨‍💻 Author
Ashutosh Kumar

GitHub: Ashu4779
