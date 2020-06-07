pipeline {
	agent { label 'master'}
     options { 
    skipDefaultCheckout()
    disableConcurrentBuilds()
	     timestamps()
   }
	   
    stages {
    stage('Clear workspace') {
      steps {
        cleanWs()
      }
    }  
    stage('GitVersion ') {
      steps {
        script {
          def datas = readYaml file: 'gitversion.yml'
         
        }
      }
    }
    stage('Source Checkout') {
      steps {
        checkout scm
    }
    }
    }

}


