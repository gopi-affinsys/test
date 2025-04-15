pipeline{
    agent any
  stages{
      stage('checkout'){
          steps{
              git branch: 'main', credentialsId: 'git-deploy', url: 'https://github.com/gopi-affinsys/test/'
          }
      }
    stage('hello'){
        when { tag "*" }
        steps{    
          sh 'echo hi'
        }
    }
  }
}
