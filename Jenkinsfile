pipeline{
  agent any
  environment {
    #FULL_PATH_BRANCH = "${sh(script:'git name-rev --name-only HEAD', returnStdout: true)}"
    #GIT_BRANCH = FULL_PATH_BRANCH.substring(FULL_PATH_BRANCH.lastIndexOf('/') + 1, FULL_PATH_BRANCH.length())
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
    
