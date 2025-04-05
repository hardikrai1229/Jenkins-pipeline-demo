pipeline {
    agent any

    triggers {
        pollSCM('* * * * *') // Polls every minute
    }

    stages {
        stage('Scripted Block') {
            steps {
                script {
                    echo "Running a scripted block inside declarative pipeline..."
                    for (int i = 1; i <= 3; i++) {
                        echo "Step ${i}"
                    }
                }
            }
        }
    }
}
