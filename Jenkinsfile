pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building.. Installing dependencies'
		sh 'npm install'
		echo 'Install mocha'
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

