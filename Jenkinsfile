pipeline{
    agent any
    stages {
        stage("Build") {
            steps {
                echo "Hello World"
                sh 'git --version'
                sh 'mkdir dir1'
                sh 'touch f{1..5}'
                sh 'cp f* dir1'
                
            }
        }
    }
}   
