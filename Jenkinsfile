pipeline {
  agent any
  parameters {
    string(name: 'VERSION1', defaultValue: '', description: 'version to deploy on prod')
    choice(name: 'VERSION', choices: ['1.1.0', '1.2.0', '1.3.0'], description: 'version to deploy on prod')
    booleanParam(name: 'executeTests', defaultValue: true, description: 'Execute the tests')
  }

  stages {
    stage('Build') {
      steps {
	      echo 'Build'
        echo 'echooo'
      }
    }

    stage(' Test') {
      when {
        expression {
          params.executeTests == true
        }
      }
      steps {
        echo 'Test'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
        echo "deploying version ${params.VERSION}"
        echo "deploying version ${params.VERSION1}"
      }
    }
  }
}