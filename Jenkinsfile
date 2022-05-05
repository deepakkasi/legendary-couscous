pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'hello'
      }
    }

    stage('QA') {
      parallel {
        stage('QA') {
          steps {
            echo 'Hi iam QA'
          }
        }

        stage('QA2') {
          steps {
            echo 'hello'
          }
        }

      }
    }

    stage('Prod') {
      steps {
        echo 'prod'
      }
    }

  }
  environment {
    name = 'deepak'
  }
}