pipeline{
  agent any
  options {
    skipDefaultCheckout(true)
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
              env.GIT_BRANCH

            '''
      }
    }
  }
}
    
