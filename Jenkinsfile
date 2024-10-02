pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the Java application...'
                sh 'javac src/main/java/Sparta.java'
            }
        }
        stage('Test') {
            steps {
                echo 'Running the application...'
                sh 'java -cp src/main/java Sparta'
            }
        }
    }
}
