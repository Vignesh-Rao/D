pipeline{
  agent any
  environment {
    FULL_PATH_BRANCH = "${sh(script:'git name-rev --name-only HEAD', returnStdout: true)}"
    GIT_BRANCH = FULL_PATH_BRANCH.substring(FULL_PATH_BRANCH.lastIndexOf('/') + 1, FULL_PATH_BRANCH.length())
    TFJOB=""
    AWSJOB=""
    GCPJOB=""
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
               echo $TFJOB
               echo it is $TFJOB-$GIT_BRANCH
               if [ "$GIT_BRANCH" = "master" ]
               then
                 TFJOB="Terraform-$GIT_BRANCH"
               fi          
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
    
