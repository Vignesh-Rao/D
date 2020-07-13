pipeline{
  agent any
  environment {
    TFJOB="Terraform-$GIT_BRANCH"
    AWSJOB="AWS-$GIT_BRANCH"
    GCPJOB="GCP-$GIT_BRANCH"
  }
  stages{
    stage('S1'){ 
      environment { 
        var1 = 'value2'
       }
      steps{
         sh '''
               echo ${GIT_BRANCH.split("/")[1]}
               echo $GIT_LOCAL_BRANCH               
            '''
      }
    }
    stage('S2'){ 
      steps{
         sh '''
               echo $TFJOB
            '''
      }
    }
  }
}
    
