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
          branch 'master'
        }
        steps{
          echo "hello dev"
        }
      }
      stage('build qa'){
        when {
          branch 'master'
        }
        steps{
          echo "hello qa"
        }
      }
    }
}
