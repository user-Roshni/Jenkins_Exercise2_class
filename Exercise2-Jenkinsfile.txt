pipeline{
    agent any
    stages{
        stage('version'){
            steps{
                bat '"C:\\Users\\Admin\\AppData\\Local\\Programs\\Python\\Python312\\python.exe" --version'
            }
        }
        stage('STAGE2'){
            steps{
                bat '"C:\\Users\\Admin\\AppData\\Local\\Programs\\Python\\Python312\\python.exe" Exercise2-python.py %X_VALUE% %Y_VALUE%'
            }
        }
    }

}

