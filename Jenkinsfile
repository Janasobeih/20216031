pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                checkout scm
            }
        }

        stage('Execute Bash Script') {
            steps {
                // Make the script executable
                sh 'chmod +x list_files.sh'

                // Execute the bash script
                sh './list_files.sh'
