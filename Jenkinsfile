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
                echo 'Holla Build!'
                ./gradlew clean test jar
            }
        }
        stage('Results'){
            steps{
                echo 'Holla Results!'
            }
        }
    }
}