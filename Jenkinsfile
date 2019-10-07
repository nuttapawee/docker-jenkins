pipeline {
stages {      
  stage ('Build') {
      steps {
        echo "Running tests in a fully containerized environment..."
        sh "./test.sh"
        sh docker logs -f elasticsearch
        sh docker logs -f kibana
      }
    }
  }
}
