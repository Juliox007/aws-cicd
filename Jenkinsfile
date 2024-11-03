pipeline {


    agent any


    environment {


        BRANCH_NAME = 'main'
        GIT_URL = 'https://github.com/Juliox007/aws-cicd.git'
        IMAGE_TAG = 'awscicd'
        IMAGE_VERSION = "${BUILD_NUMBER}"
   
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

        }

        stage('git checkout'){
            steps{
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
            }
        }


       
       stage('docker build'){
        steps{
            sh 'docker build -t "${IMAGE_TAG}:${IMAGE_VERSION}" .'
            sh 'docker images'
        }
       }
        



        stage('code'){
            steps{
                sh 'echo code'
            }
        }
    }
}
