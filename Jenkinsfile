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
            
                archiveArtifacts artifacts: 'build/libs', fingerprint: true
                junit '**/build/test-results/test/TEST-*.xm'
            }
        }
    }
}