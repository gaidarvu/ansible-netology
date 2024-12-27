pipeline {
    agent {
        label 'ansible'
    }
    stages {
        stage('Choose Dir') {
            steps {
                dir('hw-ansible-02/playbook/roles/vector')
                echo 'Change dir hw-ansible-02/playbook/roles/vector'
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