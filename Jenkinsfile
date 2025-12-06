pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/YOUR-USERNAME/ansible-cicd-project.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'ansible-playbook -i inventory playbooks/install-deps.yml'
            }
        }

        stage('Deploy Application') {
            steps {
                sh 'ansible-playbook -i inventory playbooks/deploy.yml'
            }
        }

        stage('Start Service') {
            steps {
                sh 'ansible-playbook -i inventory playbooks/start-service.yml'
            }
        }
    }
}
