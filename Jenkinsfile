pipeline {
    agent any
    stages{
      stage('build master'){
        when {
          branch 'master'
        }
        steps{
          echo "hello master"
        }
      }
      stage('build dev'){
        when {
          branch 'dev'
        }
        steps{
          echo "hello dev"
        }
      }
      stage('build qa'){
        when {
          branch 'qa'
        }
        steps{
          echo "hello qa"
        }
      }
    }
}
