pipeline {
    agent any

    stages{
        stage ('build'){
            steps{
                sh 'echo build'
            }
            
        }
        stage('test'){
            steps{
                sh 'echo test'
            }
        stage('git checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/Juliox007/aws-cicd.git'
            }
        }
        stage('code'){
            steps{
                sh 'echo code'
            }
        }
    }
}