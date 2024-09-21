pipeline {
    agent any
    environment {
        BRANCH_NAME = 'main'
        GIT_URL = 'https://github.com/Juliox007/aws-cicd.git'
    }

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
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
            }
        }
        stage('code'){
            steps{
                sh 'echo code'
            }
        }
    }
}
