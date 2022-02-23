pipeline {
    agent any

    environment {
        NEXT_VERSION = nextVersion()
    }
    stages {
        stage('Hello') {
            steps {
                echo "Next Version:: ${NEXT_VERSION}"
                echo 'Hello World'
            }
        }
        
        stage("Build") {

      steps {
           container("maven-build") {
                script {
                  sh "mvn -B clean package"
                }
              }
            } 
          } // steps
        } // stage("Build")
    }
    
    
}
