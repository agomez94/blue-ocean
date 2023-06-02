pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing'
          }
        }

        stage('Parallel') {
          steps {
            echo 'Parrallel'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'set build'
      }
    }

    stage('Clean Up') {
      steps {
        echo 'clean up complete'
      }
    }

  }
}