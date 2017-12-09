

pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello hema im downstream'              
            }
           
        }
        
       
    }
    post { 
        always { 
            echo 'I will always      say Hello again!'
            
        }
    }
}
