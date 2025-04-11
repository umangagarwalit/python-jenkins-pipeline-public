pipeline {
    agent any
    
    stages {
	
        stage('Checkout Code') {
            steps {
                git url: 'https://github.com/umangagarwalit/python-jenkins-pipeline-public.git'
            }
        }

        stage('Install Python & Dependencies') {
            steps {
                bat 'python -V'
            }
        }

        stage('Run Python Script') {
            steps {
                bat 'python python_code.py'
            }
        }
    }
}
