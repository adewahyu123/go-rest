pipeline {
  agent {
    node {
      label 'cf-sample'
    }
    
  }
  stages {
    stage('Deploy To CF') {
      steps {
        pushToCloudFoundry(target: 'api.run.pivotal.io', organization: 'Releng-Devops', cloudSpace: 'development', credentialsId: 'cf-id-1', pluginTimeout: 240)
      }
    }
  }
}