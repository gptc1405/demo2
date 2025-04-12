pipeline{
    agent any
    stages{
        stage('clone repo'){
            steps{
                git url :  'https://github.com/gptc1405/demo2.git'
            }

        }
        stage('compile java'){
            steps{
                sh ' java hello.java'
            }

        }
        stage('run java'){
            steps{
                sh 'java hello'
            }
        }
    }
}
          