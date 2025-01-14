pipeline {
    agent any 
    stages {
        stage('Clone the repo') {
            steps {
                echo 'clone the repo'
                sh 'rm -fr webapp1'
                sh 'git clone https://github.com/bickyz/webapp1.git'
            }
        }
        stage('push repo to remote host') {
            steps {
                echo 'connect to remote host and pull down the latest version'
                sh 'ssh rgsadmin@10.1.10.96 git -C /home/rgsadmin/abdocker1/webapp1 pull'
            }
        }
        stage('Stage 3') {
            steps {
                echo 'stage three here'

            }
        }
    }
}
