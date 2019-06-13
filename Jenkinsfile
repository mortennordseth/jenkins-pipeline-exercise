pipeline {
    agent any
    
    stages {
        stage('Preparation') {
            steps{
                echo 'Holla Preparation!'
            }
        }
        stage('Build') {
            steps{
                sh './gradlew clean test jar'
            }
        }
        stage('Results'){
            steps{
                echo 'Holla Results!'
            }
        }
    }
}