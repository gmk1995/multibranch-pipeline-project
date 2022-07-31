pipeline{
    agent any
    stages {
        stage("Build") {
            steps {
                echo "Hello World"
                sh 'yum install tree -y'
                sh 'tree --version'    
            }
        }
        stage("fix branch") {
          when {
            branch "fix-*"
          }
          steps {
            sh '''
              cat README.md
            '''
          }
         }
         stage("PR branch") {
          when {
            branch "PR-*"
          }
          steps {
            echo 'Runs only for PRs'        
           }
          }
    }
}
