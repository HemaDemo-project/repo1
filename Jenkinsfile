

pipeline {
    agent any
    parameters {
        booleanParam(defaultValue: true, description: '', name: 'userFlag')
    }
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
