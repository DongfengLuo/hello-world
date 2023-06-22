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
		sh "mkdir build && de build"
		sh "cmake .."
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