pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/Praveen2664/sample-web-app.git'
            }
        }

        stage('Run Ansible Playbook') {
            steps {
                sh '''
                    pwd
                    ls -l
                    ansible-playbook -i hosts.ini deploy.yml
                '''
            }
        }
    }
}

