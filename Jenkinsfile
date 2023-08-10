pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from your Git repository
                sh "pwd"
                sh "whoami"
                sh "echo '2f3308d349004e8d9e923eb04ae4938d' | sudo -S bash /home/ubuntu/remove_artifacts"
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
