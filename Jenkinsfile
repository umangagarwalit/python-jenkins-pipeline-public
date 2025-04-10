pipeline {
    agent any
    
    stages {
	
        stage('Checkout Code') {
            steps {
                git url: 'https://github.com/umangagarwalit/python-jenkins-pipeline-public.git', branch: 'main'
            }
        }

        stage('Install Python & Dependencies') {
            steps {
                sh 'python -V'
            }
        }

        stage('Run Python Script') {
            steps {
                sh 'python python_code.py'
            }
        }
    }
}
