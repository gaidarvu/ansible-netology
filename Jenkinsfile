pipeline {
    agent {
        label 'molecule'
    }
    stages {
        stage('Choose Dir') {
            steps {
                dir('hw-ansible-02/playbook/roles/vector')
            }
        }
        stage('Run Molecule Test') {
            steps {
                sh 'molecule test'
            }
        }
    }
    post {
        always {
            echo 'Pipeline Ended'
        }
    }
}