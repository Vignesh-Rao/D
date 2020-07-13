pipeline{
  agent any
  
  stages{
    stage('S1'){ 
      steps{
         sh '''
              echo $BRANCH_NAME
              echo $GIT_BRANCH
            '''
      }
    }
  }
}
    
