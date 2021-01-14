pipeline {
  agent {
    kubernetes {
      yamlFile 'deployment.yaml'
    }
  }
  stages {
    stage('Run maven') {
       steps {
       sh "echo finish"}
    }
  }
}
