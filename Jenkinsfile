pipeline{
  agent any
  environment {
    TFJOB="Iac-Terraform"
    AWS="AWS-CATALOGS"
    GCP="GCP-CATALOGS"
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
               a="${GIT_BRANCH#*/}"
               if [ "$a" = "master" ]
               then
                 a="PRD"
               fi
               echo $a
               echo "$AWS-$a"
               
            '''
      }
    }
  }
}
    
