pipeline{
  agent any
 
  stages{
    stage('S1'){ 
      steps{
         sh '''
               printenv
               echo "in s1"
               b=$GIT_BRANCH
               echo $b | cut -d "\/" -f 2
              echo "${GIT_BRANCH##*/ }"
            '''
      }
    }
  }
}
    
