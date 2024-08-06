pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'to plan the application devlopment'
      }
    }

    stage('code') {
      steps {
        echo 'developers devlop the code'
      }
    }

    stage('bulid') {
      parallel {
        stage('bulid') {
          steps {
            echo 'The code should be build'
          }
        }

        stage('Test') {
          steps {
            echo 'The code should be test'
          }
        }

        stage('delpoy') {
          steps {
            echo 'the code should be depoly'
          }
        }

        stage('operate') {
          steps {
            echo 'We can access the applicationn'
          }
        }

      }
    }

  }
}