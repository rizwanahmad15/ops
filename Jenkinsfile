pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from your Git repository
                sh "git clone https://github.com/rizwanahmad15/ops.git"
            }
        }
        
        stage("Publish Artifacts Development") {
            steps {
                sh "echo ls -al"
                sh "ssh ubuntu@18.224.88.112 rm -rf /var/www/html/*"
                // sh "scp -r ./* $USER@$DEVELOPMENT_HOST:$TARGET_PATH"
                // sh "scp -r /home/jenkins/env_vars/kwik_trust_backend $USER@$DEVELOPMENT_HOST:$TARGET_PATH/.env"
            }
        } 
    }
}
