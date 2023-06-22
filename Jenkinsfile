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
		sh "cd build"
		sh "ls"
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