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
    stage('fix branch') {
          when {
          branch 'fix-*'
          }
          steps {
          sh * * *
          cat README.md
          * * * 
          }
        }
        stage('PR branch') {
          when {
          branch 'PR-*'
          }
          steps {
          echo 'Run only for PRs'
          }
        }
}   
