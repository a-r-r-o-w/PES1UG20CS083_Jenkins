pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Starting Build'
                sh 'make -C main'
                echo 'Build Completed'
            }
        }
        stage('Test') {
            steps {
                echo 'Starting Testing'
                sh '/var/jenkins_home/workspace/PES1UG20CS083-1/main/hello_exec'
                echo 'Test Completed'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Starting Deploy'
                echo 'Deploy Completed'
		thisshoulddefinitelycauseacrash
            }
        }
    }
  post {
    failure {
      echo 'Pipeline Failed'
    }
  }
}
