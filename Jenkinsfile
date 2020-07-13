pipeline{
  agent any
  options {
    skipDefaultCheckout(true)
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
               printenv
               echo "in s1"
            '''
      }
    }
  }
}
    
