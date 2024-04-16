pipeline {
  agent {
    docker {
      image 'paulex10/androidsdk-gradle-mpos:v1.0'
    }
  }

  environment {
    PLASTICSCM_WORKSPACE_NAME = "${env.ANDROID_HOME}"
  }

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