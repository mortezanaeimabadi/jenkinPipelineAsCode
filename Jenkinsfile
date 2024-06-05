pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'building application with env variable var1 = ${var1}'
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
  environment {
    var1 = 'var1 value'
  }
}