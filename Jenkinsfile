pipeline {
    agent any
    stages {
        stage('Deploy to Kubernetes') {
            steps {
                script {
                    // Deploy to Kubernetes using kubectl
                    kubernetesDeploy(
                        configs: 'nginx-deployment.yaml',
                        kubeconfigId: 'Kubernetes'  // Replace with your Jenkins credential ID
                    )
                }
            }
        }
    }
}
