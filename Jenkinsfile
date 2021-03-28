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
                echo "Database engine is ${BRANCH_NAME}"        
        when {
          expression {
            BRANCH_NAME == 'main'
          }
        }
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
     }
    } 
