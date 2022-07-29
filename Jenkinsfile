pipeline{
    agent any
    stages {
        stage("Build") {
            steps {
                echo "Hello World"
                sh 'git --version'
                sh 'ls -al /home/jenkins'
                sh 'cd /opt'
            }
        }
    }
}   
