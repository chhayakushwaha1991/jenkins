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
       input {
                message "Should we continue?"
                ok "Yes, we should."
                submitter "alice,bob"
                parameters {
                    string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
                }
            }
      steps {
        echo "hello $name"
         echo "Hello ${params.PERSON}"
          echo "Choice: ${params.COURSE}"
        
      }
    }

    stage('stage') {
      steps {
        echo 'i am from nagpur'
      }
    }

  }
  
}
