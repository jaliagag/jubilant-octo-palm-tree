pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building in progress...'
            sh 'echo "Hello World!"'
          }
        }

        stage('Test') {
          steps {
            echo 'Unit Test in progress'
            sleep 3
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying App'
      }
    }

  }
}