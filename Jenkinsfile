pipeline {
  agent {
    dockerfile {
      filename '/root/cicd-pipeline/Dockerfile'
    }

  }
  stages {
    stage('build') {
      steps {
        sh '''/root/cicd-pipeline/scripts/build.sh
'''
      }
    }

    stage('test') {
      steps {
        sh '''/root/cicd-pipeline/scripts/test.sh
'''
      }
    }

  }
  environment {
    tinasimage = ''
  }
}