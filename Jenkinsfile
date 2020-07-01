pipeline {
    agent any
    environment {
        DATE = "${env.BUILD_TIMESTAMP}"
    }
    parameters {
        choice(choices: ['dev', 'qa', 'master'], description: 'Choose your branch?', name: 'BRANCH')
    }
    
    stages {
        stage(Githubclone){
            steps {
                   git credentialsId: 'b5391243-fa5a-4198-b2d2-c1aff1ca5288', url: 'https://github.com/chauhan1986/Test.git'
                   sh 'echo "$BRANCH"' 
            }
        }
       
        stage("mvn"){
           steps {
           sh 'mvn clean package'
           junit '**/target/surefire-reports/TEST-*.xml'
           }
        }
    }
}    
