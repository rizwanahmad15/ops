pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from your Git repository
                sh "pwd"
                sh "sudo rm -rf /var/lib/jenkins/workspace/ops_master"
                sh "sudo rm -rf /var/lib/jenkins/workspace/ops_master@tmp"
                sh "git clone https://github.com/rizwanahmad15/ops.git"
            }
        }
        
        stage("Publish Artifacts Development") {
            steps {
                sh "ls -al"
                // sh "sudo cp -R "
                // sh "scp -r ./* $USER@$DEVELOPMENT_HOST:$TARGET_PATH"
                // sh "scp -r /home/jenkins/env_vars/kwik_trust_backend $USER@$DEVELOPMENT_HOST:$TARGET_PATH/.env"
            }
        } 
    }
}
