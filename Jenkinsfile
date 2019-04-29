 pipeline {
  agent any
  options {
    buildDiscarder(logRotator(numToKeepStr: '10'))
  }
  environment {
    DOCKER_CREDS = credentials('amazeeiojenkins-dockerhub-password')
    COMPOSE_PROJECT_NAME = "drupaltest-${BUILD_ID}"
  }
  stages {
    stage('Docker login') {
      steps {
        sh """
        ls -al
        """
      }
    }
  }
}
