pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from your Git repository
                sh "pwd"
                sh "whoami"
                COMMIT_HASH = sh(script: "git log -n 1 --pretty=format:'%H'", returnStdout: true)
                sh "echo '2f3308d349004e8d9e923eb04ae4938d' | sudo -S mkdir ./${COMMIT_HASH}"
                sh "git clone https://github.com/rizwanahmad15/ops.git ./${COMMIT_HASH}"
            }
        }
        
        stage("Publish Artifacts Development") {
            steps {
                sh "echo '2f3308d349004e8d9e923eb04ae4938d' | sudo -S cp -R ./${COMMIT_HASH}/ops/* /var/www/html/."
            }
        } 
    }
}
