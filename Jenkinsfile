pipeline {
    agent any
    
    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/ThienNoob/test-jenkins.git'
            }
        }
        
        stage('Build') {
            steps {
                // Thực hiện build ở đây, ví dụ:
                sh 'npm install' // Nếu sử dụng npm
                sh 'npm run build' // Nếu sử dụng npm
                // Hoặc thực hiện bất kỳ lệnh nào để build file index.html
            }
        }
        
        stage('Test') {
            steps {
                // Thực hiện các bước kiểm thử ở đây, ví dụ:
                sh 'npm test' // Nếu sử dụng npm
                // Hoặc thực hiện các lệnh kiểm thử khác
            }
        }
        
        stage('Deploy') {
            steps {
                // Thực hiện các bước triển khai ở đây, ví dụ:
                // Copy file index.html đến thư mục cần thiết
                sh 'cp index.html /path/to/deployment/folder'
                // Hoặc sử dụng các công cụ triển khai như AWS S3, FTP, etc.
            }
        }
    }
}
