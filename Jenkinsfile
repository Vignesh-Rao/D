pipeline{
  agent any
  environment{
    TFJOB="Iac-Terraform"
    FILE_NAME="${sh(script:'($GIT_BRANCH)', returnStdout: true).trim()}"
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
               echo $FILE_NAME
               TFJOB = $TFJOB+""+FILE_NAME
            '''
      }
    }
  }
}
    
