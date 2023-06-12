pipeline {
    agent { 
        node {
            label 'docker-agent-python'
            }
      }
    triggers{
        pollSCM '*/5 * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh '''
                echo "prova test"
                echo "doing build a lot of stuff.."
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                echo "doing a lot of test stuff.."
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing a lot of delivery stuff.."
                '''
            }
        }
    }
}
