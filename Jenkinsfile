pipeline {
    agent { docker { image 'ubuntu:18.04' } }
    stages {
        stage('build') {
            steps {
                sh '''
                    set -eux
                    echo Hello world
                    uname -a
                    cat /etc/lsb-release
                    pwd
                    ls -la
                    printenv
                '''
            }
        }
        stage('confirm') {
            steps {
                input "confirm the output above"
            }
        }
        stage('continue') {
            steps {
                sh 'echo continuing'
            }
        }
    }
}
