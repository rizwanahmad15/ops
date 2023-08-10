pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from your Git repository
                sh "git clone https://github.com/rizwanahmad15/ops.git"
            }
        }
        
        stage('Build') {
            steps {
                // In this example, there's no build step for HTML.
                // You might add steps here if you need to preprocess or minify your HTML.
            }
        }
        
        stage('Deploy') {
            steps {
                // Copy the HTML files to a web server or a directory accessible via HTTP.
                // This could be an FTP upload, a cloud storage sync, or copying to a web server root.
                // Adjust this step based on your deployment method.
            }
        }
    }
}
