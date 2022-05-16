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
            echo 'testing'
          }
        }

        stage('Parallel') {
          steps {
            echo 'parallel run'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'build'
      }
    }

    stage('Cleanup') {
      steps {
        echo 'cleanup'
      }
    }

  }
}