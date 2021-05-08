pipeline {
    agent {
        any
    }

    stages {
        stage('echo') {
            steps {
                echo "branch: ${env.BRANCH_NAME}"
                echo "current SHA: ${env.GIT_COMMIT}"
            }
        }
    }
}
