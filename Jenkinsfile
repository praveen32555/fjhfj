pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''printenv | sort
echo "Build"'''
        echo 'echooo'
      }
    }

    stage(' Test') {
      steps {
        echo 'Test'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}