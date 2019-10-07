pipeline {
  agent { label 'master' }
  stages {      
    stage ('Build') {
        steps {
          echo "Running tests in a fully containerized environment..."
          sh "./test.sh"
      }
    }
  }
}
