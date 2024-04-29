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
                // Đây là nơi để xây dựng (build) file index.html.
                // Ví dụ: có thể sử dụng các công cụ như npm, yarn, gulp, webpack, etc.
                sh 'npm install' // Ví dụ: cài đặt các gói npm
                sh 'npm run build' // Ví dụ: thực thi lệnh build
            }
        }
        
        stage('Test') {
            steps {
                // Đây là nơi để chạy các bước kiểm thử.
                // Ví dụ: có thể sử dụng các công cụ như Jest, Mocha, Selenium, etc.
                sh 'npm test' // Ví dụ: chạy các bài kiểm thử
            }
        }
        
        
    }
}
