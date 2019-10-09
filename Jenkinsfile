pipeline {
<<<<<<< HEAD
agent { label 'wls03' }
stages {      
  stage ('Build') {
      steps {
        echo "Running tests in a fully containerized environment..."
        sh "./test.sh"
        sh docker logs -f elasticsearch
        sh docker logs -f kibana
=======
  agent { label 'master' }
  stages {      
    stage ('Build') {
        steps {
          echo "Running tests in a fully containerized environment..."
          sh "./test.sh"
>>>>>>> cd7e342be3d2dfb530860362a3c65f35b4a7941d
      }
    }
  }
}
