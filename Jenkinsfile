pipeline{
  agent any
 
  stages{
    stage('S1'){ 
      steps{
         sh '''
               printenv
               echo "in s1"
               echo $BRANCH_NAME
              echo "${$GIT_BRANCH##*/ }"
            '''
      }
    }
  }
}
    
