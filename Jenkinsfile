pipeline {
  agent any
  stages {
    stage('Dev') {
      parallel {
        stage('Dev') {
          steps {
            echo 'this is development '
          }
        }

        stage('') {
          steps {
            sleep 2
          }
        }

      }
    }

    stage('Stg') {
      steps {
        sleep 10
        echo 'this is stage'
      }
    }

    stage('Test') {
      steps {
        sh '''date
pwd
uptime'''
      }
    }

    stage('deploy') {
      steps {
        echo 'Deployment has done'
      }
    }

  }
}