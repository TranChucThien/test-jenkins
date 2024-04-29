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
               
                sh 'npm test' // Nếu sử dụng npm
              
        }
        
        stage('Deploy') {
            steps {
               
                sh 'cp index.html /path/to/deployment/folder'
                
        }
    }
}
