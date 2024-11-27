pipeline {
    agent any
    stages {
        stage('Deploy to Kubernetes') {
            steps {
                sshagent(['KuberSSH']) {
                    sh '''
                    ssh root@192.168.176.135 "kubectl apply -f nginx-deployment.yaml"
                    '''
                }
            }
        }
    }
}
