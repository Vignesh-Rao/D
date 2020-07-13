pipeline{
  agent any
  environment {
    MY_GIT_BRANCH="${TEMP_GIT_BRANCH#*/}"
    TFJOB="Iac-Terraform-$GIT_LOCAL_BRANCH"
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
               TEMP_GIT_BRANCH=${GIT_BRANCH}
               
            '''
      }
    }
  }
}
    
