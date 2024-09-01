
# Micro-Doppler-Based-Target-Classification

## Project Overview

The **Micro-Doppler Based Target Classification** project focuses on distinguishing between different Small Aerial Targets like Drones, RC Planes, Birds, etc by analyzing micro-Doppler signatures captured from radar sensors. <br>
This technology is essential for improving situational awareness in scenarios such as surveillance, search and rescue missions, and safeguarding critical infrastructure. <br>

The project encompasses:

**Signal Processing**: Obtained dataset from IEEE Dataport, which is around 4000 spectrogram images extracted from radar data. This data is normalized, and augmented. Feature extraction is used to to extract meaningful features                           from the spectrograms, to enhance model's performance.<br>
**Machine Learning**: Implementing Python-based models to classify objects based on the extracted features.<br>
**Web Application**: Creating an intuitive interface for users to interact with the classification system.<br>


| Classes | Three-Long-Blade-Rotor | Three-Short-Blade-Rotor | Bird | Bird + Mini-Helicopter | Drone | RC Plane |
|:--------|:------------------------|:-----------------------|:-----|:-----------------------|:------|:---------:|
| Pictures | ![image](https://github.com/user-attachments/assets/7006926f-85d9-47da-8289-b3236dc158d8)| ![image](https://github.com/user-attachments/assets/fe8962c3-1660-4732-ad0e-daee44cd3e27) | ![image](https://github.com/user-attachments/assets/d396b45a-1c45-4f8c-a73e-dd0d850661f3) | ![image](https://github.com/user-attachments/assets/ab27f402-83ed-4196-aa03-f3a1727212f8) | ![image](https://github.com/user-attachments/assets/a5f9c9da-198c-42b6-a9ba-04ad240e1448) | ![image](https://github.com/user-attachments/assets/2634c1c5-a1a4-41ed-b8b2-b9b2c9111e5f) | 
| Spectrogram Images | ![image](https://github.com/user-attachments/assets/4eacd2ae-aff1-46c1-84aa-7c35b9354edd) | ![image](https://github.com/user-attachments/assets/34cf66ed-5f45-47d7-8517-eee29e4b1c48) | ![image](https://github.com/user-attachments/assets/7d45fd48-19a1-4bec-83ad-53cb37fb72d9) | ![image](https://github.com/user-attachments/assets/7c335c47-f2a2-41fe-b9b7-02faae0e542b) | ![image](https://github.com/user-attachments/assets/51c2aa8f-cac6-4436-8c13-da3fed6cd21a) | ![image](https://github.com/user-attachments/assets/3da26ff9-8eb9-4fa4-a9e5-fb9c5329b55c) | 










 



## Contributors 

**[Inchara J](https://github.com/Incharajayaram)**<br>

**[Shravya H Jain](https://github.com/shravya312)**<br>

**[Diptangshu Bej](https://github.com/DiptangshuBej)**<br>

**[Anand Raut](https://github.com/Anand-Raut9)**<br>

**[Likith Manjunatha](https://github.com/Likith-m-22)**<br>

**[Chethan A C](https://github.com/chethanac15)**<br>

## Tech Stack

**Frontend**: React, HTML, Bootstrap, JavaScript.<br>

**Backend**: Flask/Express.js.<br>

**Machine Learning**: Python, PyTorch, Scikit-learn, numpy.<br>

**Visualization**: Matplotlib.<br>

**Deployment**: Docker, Gunicorn.<br>

**Version Control & CI/CD**: Git/GitHub, GitHub Actions.<br>

## Project Structure

```sh
Micro-Doppler-Based-Target-Classification-/
├── Frontend/                      # React frontend directory
│   ├── public/                    # Public assets like HTML, icons, etc.
│   ├── src/
│   │   ├── assets/                # Static assets (images, fonts, etc.)
│   │   ├── components/            # Reusable React components
│   │   ├── pages/                 # Page components (Home, Dashboard, etc.)
│   │   ├── services/              # API calls to Flask backend
│   │   ├── App.js                 # Main React component
│   │   ├── index.js               # React entry point
│   │   └── styles/                # CSS/Sass files
│   ├── .env                       # Environment variables
│   ├── package.json               # NPM dependencies
│   └── README.md                  # Frontend documentation
├── Backend/                       # Flask backend directory
│   ├── app/
│   │   ├── __init__.py            # Flask app initialization
│   │   ├── controllers/           # Route controllers
│   │   │   ├── classification.py  # Classification API endpoint
│   │   │   ├── healthcheck.py     # Healthcheck API endpoint
│   │   ├── models/                # Data models (if needed)
│   │   ├── services/              # Business logic (model inference, etc.)
│   │   │   ├── model_inference.py # Logic for loading models and making predictions
│   │   ├── utils/                 # Utility functions (e.g., logging, error handling)
│   │   ├── static/                # Static files (model weights, logs)
│   │   ├── templates/             # HTML templates (if needed for serving static pages)
│   │   └── config.py              # Configuration file (for environment variables, etc.)
│   ├── tests/                     # Unit tests for backend
│   │   ├── test_classification.py # Tests for the classification endpoint
│   │   └── conftest.py            # Test configurations and fixtures
│   ├── requirements.txt           # Python dependencies
│   ├── wsgi.py                    # WSGI entry point for production (optional)
│   ├── .flaskenv                  # Flask-specific environment variables
│   ├── .env                       # General environment variables
│   └── README.md                  # Backend documentation
├── ml_model/                      # Machine learning model directory
│   ├── notebooks/                 # Jupyter notebooks for experiments and model training
│   ├── src/
│   │   ├── data/                  # Data handling scripts
│   │   ├── model/                 # Model training, evaluation, and prediction scripts
│   │   ├── utils/                 # Utility scripts (data preprocessing, visualization)
│   │   ├── main.py                # Main script python file to run the pretrained moddel
│   ├── requirements.txt           # Python dependencies for ML
│   ├── venv/                      # Virtual environment for ML
│   ├── .gitignore                 # Ignore unnecessary files (e.g., model weights, virtual env)
│   └── README.md                  # ML model documentation
├── docker-compose.yaml            # Docker Compose file (if containerizing)
├── Dockerfile                     # Dockerfile for backend (if containerizing)
├── .gitignore                     # Global .gitignore file
├── LICENSE                        # License file
└── README.md                      # Main project documentation
```

## Contributing

1. **Fork the repository**
2. **Create a new branch**:

   ```sh
   git checkout -b feature
   ```

3. **Make your changes**
4. **Add your changes**:-

   ```sh
   git add <filename>
   ```
5. **Commit your changes**:

   ```sh
   git commit -m 'Add new feature'
   ```

6. **Push to the branch**:

   ```sh
   git push origin feature
   ```

7. **Create a new Pull Request**
