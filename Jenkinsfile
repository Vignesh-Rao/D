pipeline{
  agent any
  environment {
    FILE_NAME="${sh(script:'($GIT_BRANCH)', returnStdout: true).trim()}"
    TFJOB="Iac-Terraform"
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
               echo hi
            '''
      }
    }
  }
}
    
