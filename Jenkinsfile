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
        when {
          expression {
                            echo "Database engine is ${BRANCH_NAME}"        

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
