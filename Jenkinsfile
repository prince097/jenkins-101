pipeline {
    agent any
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                bat 'python --version'
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                bat 'helloworld.py'
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                echo "doing delivery stuff.."
                
            }
        }
    }
}
