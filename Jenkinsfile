pipeline {
  agent any

  stages {
    stage('assemble-topwise-dev') {
      steps {
        sh "echo 'emem pipeline' "
        sh 'touch local.properties'
        sh 'printenv'
        echo "Running Boy ${env.PLASTICSCM_WORKSPACE_NAME}"
        sh "echo sdk.dir=/android-home >> local.properties"
        sh "ls /android-home"
      }
    }

  }
}