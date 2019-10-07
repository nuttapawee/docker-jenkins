pipeline {
stages {      
  stage ('Build') {
      steps {
        echo "Running tests in a fully containerized environment..."
        sh "./test.sh"
        sudo docker logs -f elasticsearch
        sudo docker logs -f kibana
      }
    }
  }
}
