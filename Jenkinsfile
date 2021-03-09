pipeline {
    agent any
    stages {
        
        
        stage('Compile') {
            steps{
                 bat 'dir'
            }
        }
    }
    post {
        failure {
            mail bcc: '', body: "$BUILD_NUMBER", subject: "$JOB_NAME", to: 'machhirke_atitkumar.ghrcecs@raisoni.net'
        }
        success {
            mail bcc: '', body: "$BUILD_NUMBER", subject: "$JOB_NAME", to: 'machhirke_atitkumar.ghrcecs@raisoni.net'
        }      
    }
}