pipeline {
  agent any
  stages {
    stage('Prepare environment') {
      steps {
        sh 'jenkins_scripts/prepare.sh'
      }
    }
    stage('Test Config') {
      steps {
        sh 'jenkins_scripts/test.sh'
      }
    }
    stage('Deploy') {
      steps {
        sh 'jenkins_scripts/deploy.sh'
      }
    }
  }
}

