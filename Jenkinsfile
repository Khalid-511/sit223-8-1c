pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Khalid-511/sit223-8-1c.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application... (Tool: Maven or npm)'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit & integration tests... (Tools: JUnit, Mocha)'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Analysing code quality... (Tool: SonarQube)'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Scanning for vulnerabilities... (Tool: Snyk / OWASP Dependency Check)'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to staging environment... (Tool: Jenkins to EC2/Docker)'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Running staging integration tests... (Tools: Selenium, Postman)'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Deploying to production... (Tool: Jenkins + AWS/Kubernetes)'
            }
        }
    }
}
