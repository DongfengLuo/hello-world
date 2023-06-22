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
		sh "mkdir build"
		sh "ls"
      }
    }

    stage('Build') 
    {
      agent any
      steps 
      {
	  dir('build'){
		echo 'Start Build..'
		sh "ls"
		sh "cmake ../"
		sh "make"
		}
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