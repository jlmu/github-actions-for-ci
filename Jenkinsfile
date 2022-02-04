pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sleep 5
        sh 'echo "building"'
      }
    }

    stage('firefox') {
      parallel {
        stage('firefox') {
          steps {
            sh 'echo "firefox here"'
          }
        }

        stage('edge') {
          steps {
            echo 'edge here'
          }
        }

      }
    }

    stage('close') {
      steps {
        sleep 3
        echo 'closing...'
      }
    }

  }
}