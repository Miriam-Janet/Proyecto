pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		sh 'npm install'
		sh 'npm install --global mocha'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                   sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}

