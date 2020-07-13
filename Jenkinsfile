pipeline{
  agent any
  options {
    skipDefaultCheckout(true)
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
              echo $BRANCH_NAME

            '''
      }
    }
  }
}
    
