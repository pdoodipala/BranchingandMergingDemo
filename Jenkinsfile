node
  {
  stage('checkout')
    {
    checkout scm
    }
  stage('Main PR')
    {
    echo 'branch name ' + env.BRANCH_NAME
      
    if (env.BRANCH_NAME.startsWith("master"))
      {
      echo "Deploying to PROD environment"
      }
      
    sh """chmod +x HelloWorld.sh 
    ./HelloWorld.sh"""
 
    }
  }
