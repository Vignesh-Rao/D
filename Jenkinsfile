pipeline{
  agent any
  options {
    skipDefaultCheckout(true)
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
               echo 'Pulling...' + env.BRANCH_NAME
               echo "in s1"
            '''
      }
    }
  }
}
    
