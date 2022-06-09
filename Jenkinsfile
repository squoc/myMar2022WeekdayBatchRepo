pipeline {
    agent any
    
    stages {
        stage('checkout-scm') {
            steps {
                build job: 'checkout-scm'
            }
        }
        
        stage('build') {
            steps {
                build job: 'maven-build'
            }
        }
        
        stage('deploy') {
            steps {
                build job: 'deploy'
            }
        }
    }
}
