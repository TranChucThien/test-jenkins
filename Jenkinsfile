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
               
                sh 'npm install' // Ví dụ: cài đặt các gói npm
                sh 'npm run build' // Ví dụ: thực thi lệnh build
            }
        }
        
        stage('Test') {
            steps {
               
                sh 'npm test' // Ví dụ: chạy các bài kiểm thử
            }
        }
        
        
    }
}
