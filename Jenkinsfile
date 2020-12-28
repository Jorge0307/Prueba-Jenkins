pipeline {
  agent {
    kubernetes {
      yamlFile 'examples/declarative_from_yaml_file/KubernetesPod.yaml'
    }
  }
  stages {
  stage "Deploy"

        sh "sed 's#__IMAGE__#'$BUILDIMG'#' part1/hello-kenzan/k8s/deployment.yaml | kubectl apply -f -"
}
}
