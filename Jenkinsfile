pipeline {    
stages('Build') {
    steps {
      echo "Running tests in a fully containerized environment..."
      dir ('test-scripts') {
        sh "./test.sh"
        sh docker logs -f elasticsearch
        sh docker logs -f kibana
      }
    }
  }
}
