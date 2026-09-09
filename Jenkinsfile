pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Bhavatharene12/list_utilities_project.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat '"C:\\Users\\bhava\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" -m pip install -r requirements.txt'
            }
        }

        stage('Run Unit Tests') {
            steps {
                bat '"C:\\Users\\bhava\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" -m pytest test_app.py -v'
            }
        }
    }
}