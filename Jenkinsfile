pipeline {
    agent any
    
    stages {
        
        stage('build & package') {
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
