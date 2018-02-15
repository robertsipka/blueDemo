pipeline {
  agent any
  parameters {
    choice (name: 'role_choice',
      choices: 'master\nslave\n',
      description: 'What role do you choose?')
    booleanParam(name: 'CAN_EXECUTE',
      defaultValue: true,
      description: 'Checkbox parameter')
  }
  stages {
    stage('Example') {
      steps {
        echo 'Hello World!'
        echo "Selected role: ${params.role_choice}"
        echo "It can execute: ${params.CAN_EXECUTE}"
      }
    }
  }
}
