pipeline{
  agent any 
  stages{
    stage ("Maven Build"){
      when{
        branch 'develop'
      }  
      steps{
        echo "maven build........."
      }
    }
    stage ("Sonar Analysis"){
      when{
        branch 'develop'
      }  
      steps{
        echo "Sonar Analysis........."
      }
    }
    stage ("Deploy to Dev"){
      when{
        branch 'develop'
      }  
      steps{
        echo "deploying to development........."
      }
    }
    stage ("Deploy to QA"){
      when{
        branch 'test'
      }  
      steps{
        echo "deploying to QA........."
      }
    }
    stage ("Deploy to Prod"){
      when{
        branch 'main'
      }  
      steps{
        echo "deploying to Prod........."
      }
    }
  }
 } 
