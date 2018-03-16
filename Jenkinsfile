pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'this is the build stage'
      }
    }
    stage('DeployTo-A') {
      parallel {
        stage('DeployTo-A') {
          steps {
            echo 'This will deploy to env A'
          }
        }
        stage('Deployto-B') {
          steps {
            echo 'This will deploy to B'
          }
        }
      }
    }
  }
}