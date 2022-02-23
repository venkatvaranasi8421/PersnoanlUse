pipeline {
    agent any
    tools { 
        maven 'maven-path'
    }
    environment {
        NEXT_VERSION = nextVersion(writeVersion: true)
    }
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
            }
        }

        stage ('Build') {
            steps {
                echo "next version = ${NEXT_VERSION}"
                echo 'This is a minimal pipeline.'
            }
        }
    }
}
