pipeline {
    agent any

    triggers {
        pollSCM('H/2 * * * *')
    }

    stages {
        stage('Stage 1: Build') {
            steps {
                echo 'Task: Build the code by compiling and packaging the application.'
                echo 'Tool: Maven, Gradle, or npm can be used as build automation tools.'
            }
        }

        stage('Stage 2: Unit and Integration Tests') {
            steps {
                echo 'Task: Run unit tests to ensure the code functions as expected.'
                echo 'Task: Run integration tests to ensure different components work together.'
                echo 'Tool: JUnit, Jest, Mocha, or Selenium can be used for test automation.'
            }
        }

        stage('Stage 3: Code Analysis') {
            steps {
                echo 'Task: Analyse the code and check whether it meets industry standards.'
                echo 'Tool: SonarQube, SonarCloud, or Checkstyle can be used for code analysis.'
            }
        }

        stage('Stage 4: Security Scan') {
            steps {
                echo 'Task: Perform a security scan to identify vulnerabilities in the code.'
                echo 'Tool: Snyk, npm audit, OWASP Dependency-Check, or Trivy can be used for security scanning.'
            }
        }

        stage('Stage 5: Deploy to Staging') {
            steps {
                echo 'Task: Deploy the application to a staging server.'
                echo 'Tool: AWS EC2, Docker, Kubernetes, or Jenkins deployment scripts can be used.'
            }
        }

        stage('Stage 6: Integration Tests on Staging') {
            steps {
                echo 'Task: Run integration tests on the staging environment.'
                echo 'Tool: Selenium, Postman/Newman, or Cypress can be used for staging tests.'
            }
        }

        stage('Stage 7: Deploy to Production') {
            steps {
                echo 'Task: Deploy the application to a production server.'
                echo 'Tool: AWS EC2, Kubernetes, Docker, or Ansible can be used for production deployment.'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully.'
        }
        failure {
            echo 'Pipeline failed. Please check the console output.'
        }
    }
}