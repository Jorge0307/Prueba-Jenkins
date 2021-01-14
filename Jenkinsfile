pipeline {
  agent {
    kubernetes {
      yamlFile 'deployment.yaml'
    }
  }
stages {
    stage('Run') {
      steps { sh "echo hola"}
    }
}
      }
