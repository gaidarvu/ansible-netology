pipeline {
    agent {
        label 'ansible'
    }
    stages {
        stage('Choose Dir') {
            steps {
                sh 'cd hw-ansible-02/playbook/roles/vector'
                sh 'ls -lad'
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