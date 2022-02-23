pipeline {
    agent any
    tools { 
        maven 'maven-path'
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
                def NextVersion = nextVersion()
                def CurrentVersion = currentVersion()
                echo 'Current Version: $[CurrentVersion}'
                echo 'Next Version: ${NextVersion}'
                echo 'This is a minimal pipeline.'
            }
        }
    }
}
