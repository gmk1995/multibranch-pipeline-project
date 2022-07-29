pipeline{
    agent any
    stages {
        stage("Build") {
            steps {
                echo "Hello World"
                sh 'git --version'
                sh 'cat /etc/os-release'
                sh 'cd /opt'
            }
        }
    }
}   
