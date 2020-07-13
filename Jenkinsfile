pipeline{
  agent any
  environment{
    TFJOB="Iac-Terraform"
    FILE_NAME="${sh(script:'(echo $GIT_BRANCH | cut -d'/' -f2)', returnStdout: true).trim()}"
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
               echo $FILE_NAME
               echo $TFJOB
               TFJOB = $TFJOB-$FILE_NAME
               echo $TFJOB
            '''
      }
    }
  }
}
    
