pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                dir("node"){
                   sh 'npm install'
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                 dir("node"){
                   sh 'npm test'
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
