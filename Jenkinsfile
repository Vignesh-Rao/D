pipeline{
  agent any
 
  stages{
    stage('S1'){ 
      steps{
         sh '''
               printenv
               echo "in s1"
               b=echo $GIT_BRANCH
               echo "${b##*/ }"
              echo "${GIT_BRANCH##*/ }"
            '''
      }
    }
  }
}
    
