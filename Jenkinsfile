pipeline
{
  agent any

  stages 
  {
    stage('Prepare') 
    {
      steps 
      {
        echo 'Start Pipeline..'
      }
    }

    stage('Build') 
    {
      agent any
      steps 
      {
		echo 'Start Build..'
		sh "ls"
		sh "mkdir build"
		sh "ls"
		sh "cd ./build"
		sh "cmake ../"
		sh "make"

      }
    } 

    stage('Package') 
    {
      steps 
      {
         echo 'packing..'
      }
    }
  
    stage('Clean..') 
    {
      steps
      {
        echo 'packing..'
      }
    }
  
  } 

} 