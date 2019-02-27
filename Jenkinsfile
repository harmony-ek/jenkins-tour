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
                '''
            }
        }
    }
}
