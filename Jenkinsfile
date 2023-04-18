pipeline {
    agent any
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                cd myapp
                pip install -r requirements.txt
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                cd myapp
                python3 hello.py
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
