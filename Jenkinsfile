

pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello hema im downstream'
              script {
                  if (env.BRANCH_NAME == 'master') {
                   build '../repo2/master'
                            }  
              }
              
            }
        }
    }
    post { 
        always { 
            echo 'I will always      say Hello again!'
        }
    }
}
