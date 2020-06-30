pipeline {
    agent any
    environment {
        DATE = "${env.BUILD_TIMESTAMP}"
    }
    parameters {
        choice(choices: ['dev', 'qa', 'enterpriseqa', 'production'], description: 'Choose your branch?', name: 'BRANCH')
    }
    
    stages {
        stage(build){
            steps {
                sh 'echo "hello"' 
            }
        }
    }
}    
