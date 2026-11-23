node {
    stage('Checkout') {
        checkout scm
    }

    stage('Verify Source Code') {
        sh 'test -f package.json'
        sh 'echo "OWASP Juice Shop source code verified successfully"'
    }

    stage('Build Status') {
        echo 'Jenkins CI pipeline completed successfully'
    }
}
