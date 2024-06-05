pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'building application'
          }
        }

        stage('Test') {
          steps {
            echo 'Testing application'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying to environment'
      }
    }

  }
}