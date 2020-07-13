pipeline{
  agent any
  options {
    skipDefaultCheckout(true)
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
               echo "*************************IN D1****************************"
               printenv
               echo "in s1"
            '''
      }
    }
  }
}
    
