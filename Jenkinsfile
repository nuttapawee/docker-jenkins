pipeline {
agent { label 'wls03' }
stages {      
  stage ('Build') {
      steps {
        echo "Running tests in a fully containerized environment..."
        sh "./test.sh"
        sh "sudo docker logs -f elasticsearch"
        sh "sudo docker logs -f kibana"
      }
    }
  }
}
