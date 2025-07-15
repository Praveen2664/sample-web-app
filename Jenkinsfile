pipeline {
    agent any

    stages {
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

