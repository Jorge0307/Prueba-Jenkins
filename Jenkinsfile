pipeline {
  agent {
    kubernetes {
      yamlFile 'examples/declarative_from_yaml_file/KubernetesPod.yaml'
    }
  }
  stages {
  stage "Deploy"

        sh "sed 's#__IMAGE__#'$BUILDIMG'#' deployment.yaml | kubectl apply -f -"
}
}
