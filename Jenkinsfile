pipeline {
  agent any
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'ciaone'
          }
        }

        stage('waiter') {
          steps {
            sleep 1
          }
        }

      }
    }

    stage('cul') {
      steps {
        echo 'culone'
      }
    }

  }
}