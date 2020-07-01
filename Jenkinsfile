pipeline {
    agent any
    environment {
        DATE = "${env.BUILD_TIMESTAMP}"
    }
    parameters {
        choice(choices: ['dev', 'qa', 'enterpriseqa', 'production'], description: 'Choose your branch?', name: 'BRANCH')
    }
    
    stages {
        stage(Githubclone){
            steps {
                sh 'echo "$BRANCH"' 
            }
        }
    }
}    
