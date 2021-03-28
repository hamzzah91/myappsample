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
        
        echo "${BRANCH_NAME}"
        when {
          expression {
            BRANCH_NAME == 'dev'
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
