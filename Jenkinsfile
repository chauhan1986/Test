pipeline {
    agent any
    
    stages {
        stage("Gitclone"){
            steps {
                git credentialsId: 'b5391243-fa5a-4198-b2d2-c1aff1ca5288', url: 'https://github.com/chauhan1986/Test.git' ,branch: "$BRANCH"
                echo "$BRANCH"
            }
        }
        stage("dev"){
            steps {
                echo "dev"
            }
        }
    }
}    
