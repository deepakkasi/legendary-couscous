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
            sh 'echo "Hi i am QA2"'
          }
        }

      }
    }

    stage('Prod') {
      steps {
        sh 'echo "Hi i am Prod stage"'
      }
    }

  }
  environment {
    name = 'deepak'
  }
}