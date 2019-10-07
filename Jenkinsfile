pipeline {
stages {      
  stage ('Build') {
      steps {
        echo "Running tests in a fully containerized environment..."
        sh "./test.sh"
        docker logs -f elasticsearch
        docker logs -f kibana
      }
    }
  }
}
