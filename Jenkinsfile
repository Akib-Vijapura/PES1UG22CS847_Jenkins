pipeline{
  agent any
  stages{
    stage("Build"){
      steps{
        build 'PES1UG22CS847-1'
        sh 'g++ hello.cpp -o hello'
      }
    }
    stage("Test"){
      steps{
        sh './iuiygd'
      }
    }
    stage("Deploy"){
      steps{
        echo 'Deploy'
      }
    }
  }
  post{
    failure{
      error 'Pipeline failed'
    }
  }
}
