pipeline {
    agent any
    environment {
        DATE = "${env.BUILD_TIMESTAMP}"
    }
    parameters {
        choice(choices: ['dev', 'qa', 'enterpriseqa', 'production'], description: 'Choose your branch?', name: 'BRANCH')
    }
    
    stages {
        stage("Gitclone"){
            steps {
                git credentialsId: 'b5391243-fa5a-4198-b2d2-c1aff1ca5288', url: 'https://github.com/chauhan1986/Test.git'
            }
        }
        stage("master"){
            steps {
                sh 'echo "master"' 
            }
        }
    }
}    
