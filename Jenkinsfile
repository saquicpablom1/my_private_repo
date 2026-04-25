pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main',
                    credentialsId: 'github-ssh-key',
                    url: 'git@github.com:saquicpablom1/my_private_repo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
    }
}
