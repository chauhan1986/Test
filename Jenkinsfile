pipeline {
    agent any
    options {
        timestamps()
    }
    stages{
      stage('build master'){
        when {
          branch 'master'
        }
         stages{
      stage('build qa'){
        when {
          branch 'qa'
        } 
            steps {
                   git credentialsId: 'b5391243-fa5a-4198-b2d2-c1aff1ca5288', url: 'https://github.com/chauhan1986/Test.git'
                   sh 'echo "$BRANCH"' 
            }
      
       
        stage("mvn"){
           steps {
           sh 'mvn clean package'
           }
        }
    }
}    
