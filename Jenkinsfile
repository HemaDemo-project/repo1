

pipeline {
    agent any
    parameters {
        booleanParam( description: '', name: 'userFlag')
        string(defaultValue: true, description: '', name: 'userString')
         // choices are newline separated
        choice(choices: 'US-EAST-1\nUS-WEST-2', description: 'What AWS region?', name: 'region')
    
    }
    stages {
        stage('Example') {
            steps {
                echo 'Hello hema im downstream'  
                 sh "echo ${params.region}"
            }
           
        }
        
       
    }
    post { 
        always { 
            echo 'I will always      say Hello again!'
            
        }
    }
}
