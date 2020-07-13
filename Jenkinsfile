pipeline{
  agent any
  options {
    skipDefaultCheckout(true)
  }
  stages{
    stage('S1'){ 
      steps{
         sh '''
               echo GIT_COMMIT %GIT_COMMIT% 
echo GIT_BRANCH %GIT_BRANCH%
echo GIT_LOCAL_BRANCH %GIT_LOCAL_BRANCH%
echo GIT_PREVIOUS_COMMIT %GIT_PREVIOUS_COMMIT%
echo GIT_PREVIOUS_SUCCESSFUL_COMMIT %GIT_PREVIOUS_SUCCESSFUL_COMMIT%
echo GIT_URL %GIT_URL%
echo GIT_URL_N - %GIT_URL_N%
echo GIT_AUTHOR_NAME %GIT_AUTHOR_NAME%
echo GIT_COMMITTER_EMAIL %GIT_COMMITTER_EMAIL%
            '''
      }
    }
  }
}
    
