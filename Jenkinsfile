pipeline{
    agent any
  stages{
    stage('hello'){
        when { tag "*" }
        steps{    
          sh 'echo hi'
        }
    }
  }
}
