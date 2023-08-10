pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from your Git repository
                sh "pwd"
                sh "bash /home/ubuntu/remove_artifacts"
                sh "git clone https://github.com/rizwanahmad15/ops.git"
            }
        }
        
        stage("Publish Artifacts Development") {
            steps {
                sh "bash /home/ubuntu/deploy_artifacts"
            }
        } 
    }
}
