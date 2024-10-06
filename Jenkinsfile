pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                // Clone the GitHub repository and specify the main branch
                git branch: 'main', url: 'https://github.com/shaid2233/jenkins.git'
            }
        }

        stage('Run main.py') {
            steps {
                // Run the Python script using the Windows command shell
                bat 'python main.py'
            }
        }
    }
}
