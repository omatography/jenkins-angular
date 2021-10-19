pipeline {
  tools {
    nodejs 'node16'
  }
    agent any
    stages {
        stage('Check version') {
            steps {
                echo 'Cleaning..'
                // bat 'npm --version'
            }
        }
        stage('Install dependencies') {
            steps {
                // echo 'Install deps..'
                // bat 'npm install'
                emailext body: 'Test Message',
                subject: 'Installed Dependancies',
                to: 'omkarrsurve21@gmail.com'
            }
        }

        stage('Test') {
            steps {
                // echo 'Testing..'
                // bat 'npm test'
                emailext body: 'Test Message',
                subject: 'Installed Dependancies',
                to: 'omkarrsurve21@gmail.com'
            }
        }
        stage('Package') {
            steps {
                echo 'npm build'
            }
        }
    }
}