pipeline{
    agent any
    stages{
        stage('clone repo'){
            steps{
                git url :  'https://github.com/gptc1405/demo2.git' , branch:'main'
            }

        }
        stage('compile java'){
            steps{
                bat 'java hello.java'
            }

        }
        stage('run java'){
            steps{
                bat 'java hello.java'
post{
    sucess{
        echo "bulid and run sucessfully"
        }
        faliure{
            echo "bulid failed"
        }
}         
            }
        }
    }
}
