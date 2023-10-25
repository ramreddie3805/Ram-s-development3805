pipeline {
  agent any
  stages {
    stage('Development') {
      steps {
        echo 'i want to develop'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'i want to build'
          }
        }

        stage('test') {
          steps {
            echo 'i want to test'
          }
        }

        stage('deploy') {
          steps {
            echo 'i want to deploy'
          }
        }

      }
    }

  }
}