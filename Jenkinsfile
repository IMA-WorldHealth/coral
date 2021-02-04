pipeline {
  agent {
    docker {
      image 'buildkite/puppeteer:latest'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'yarn'
        sh 'yarn test'
      }
    }

    stage('Finish') {
      steps {
        echo 'Done!'
      }
    }

  }
}