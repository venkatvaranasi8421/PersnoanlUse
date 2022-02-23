pipeline {
    agent any

    environment {
        NEXT_VERSION = nextVersion(writeVersion: true)
    }
    stages {
        stage('Hello') {
            steps {
                echo "Next Version:: ${NEXT_VERSION}"
                echo 'Hello World'
            }
        }
    }
}
