pipeline {
    agent any
    stages{
        stage('Checkout code'){
            steps{
                git url: 'https://github.com/CHEPURIMEGHANA/gradle-demo.git', branch: 'main'
            }
        }
        stage('Build') {
            steps{
                sh './gradlew build'
            }
        }
        stage('Run') {
            steps{
                sh './gradlew run'
            }
        }
    }
}
