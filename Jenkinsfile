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
    stage('Source Checkout') {
      steps {
        checkout scm
    }
    }
    }
