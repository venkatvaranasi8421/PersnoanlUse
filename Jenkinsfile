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
    }
}
