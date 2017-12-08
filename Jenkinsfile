

pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello hema im downstream'              
            }
            stage('2'){
                steps{
                script {
                  if (env.BRANCH_NAME == 'master') {
                   build '../repo2/master'
                            }  
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
