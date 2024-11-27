pipeline {
    agent any
    stages {
        stage('Deploy to Kubernetes') {
            steps {
                script {
                    // Deploy to Kubernetes using kubectl
                    kubernetesDeploy(
                        configs: 'nginx-deployment.yaml',
                        kubeconfigId: 'kubernetes'  // Replace with your Jenkins credential ID
                    )
                }
            }
        }
    }
}
