pipeline {
    agent any
    stages {
      stage ("clone-master") {
         when {
         branch 'master'
         }
         steps {
              git credentialsId: 'b5391243-fa5a-4198-b2d2-c1aff1ca5288', url: 'https://github.com/chauhan1986/Test.git' 
                echo "$BRANCH"
         }
         stage ("build"){
            steps {
              echo "clone master"
            }
         }


      }
      stage ("clone-qa") {
         when {
         branch 'qa'
         }
         steps {
              git credentialsId: 'b5391243-fa5a-4198-b2d2-c1aff1ca5288', url: 'https://github.com/chauhan1986/Test.git' 
                echo "$BRANCH"
         }
         stage ("build"){
            steps {
              echo "clone qa"
            }
         }


      }
      stage ("clone-dev") {
         when {
         branch 'dev'
         }
         steps {
              git credentialsId: 'b5391243-fa5a-4198-b2d2-c1aff1ca5288', url: 'https://github.com/chauhan1986/Test.git' 
                echo "$BRANCH"
         }


      }
      stage ("build"){
            steps {
              echo "clone dev"
            }
         }

    }
}
