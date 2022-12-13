pipeline {
  agent any
  environment {
    name = 'chhaya'
  }
   parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
   }
  stages {
    stage('build') {
      steps {
        echo "hello $name"
         echo "Hello ${params.PERSON}"
      }
    }

    stage('stage') {
      steps {
        echo 'i am from nagpur'
      }
    }

  }
  
}
