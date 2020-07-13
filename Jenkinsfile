pipeline{
  agent any
  environment {
    ]
    TFJOB="Iac-Terraform"
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
               echo we need to run "TFJOB-${TEMP_GIT_BRANCH#*/}"
               
            '''
      }
    }
  }
}
    
