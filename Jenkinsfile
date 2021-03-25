pipeline {
  agent any 
    stages {
      stage("build") {
      
        steps {
          echo 'building the application ... '
                    echo 'built the application ... '

        }
      }
      stage("test") {
      
        steps {
          echo 'testing the application ... '
                    echo 'tested ... '

        }
      }
      stage("deploy") {
      
        steps {
          echo 'deploying the application ... '
        }
      }
      post
      {
        always{
        echo ' always called'
        //sending an email about the build condition to the tema
        }
        success{
                  echo ' success called'
        }
        failure{
                  echo ' failure called'
        }
      }
     }
    } 
