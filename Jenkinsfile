pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                sh 'https://github.com/Amrit2055/SpartaJavaCode.git'
            }
        }
        stage('Build') {
            steps {
                //echo 'Running the application...'
                sh 'java -cp src/main/java sparta'
            }
        }
        stage('Security Scan') {
            steps {
                //echo 'Running the application...'
                sh 'dependency-check --scan ./ --out report'
            }
        }
    }
}
