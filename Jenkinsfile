pipeline{
  agent any
  environment {
    
    TFJOB="Iac-Terraform-$GIT_LOCAL_BRANCH"
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
               echo $TFJOB
            '''
      }
    }
  }
}
    
