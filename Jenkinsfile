pipeline {
    agent any
    stages{
        stage("checkout"){
            steps{
                checkout scm
            }
        }

        stage("Test"){
            steps{
                sh 'sudo apt install npm'
                sh 'sudo npm test'
            }
        }

        stage("Build"){
            steps{
                sh 'sudo npm run build'
            }
        }
    }
}
