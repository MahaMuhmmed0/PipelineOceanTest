pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building done....'
      }
    }

    stage('Test1') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing1 done....'
          }
        }

        stage('Test2') {
          steps {
            echo 'Testing2 done....'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying done....'
      }
    }

  }
}