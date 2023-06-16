pipeline {
    agent any
    customWorkspace /root/jenkins_Workspace
    stages {
        stage('CheckOut the Code) {
            steps {
                // Get some code from a GitHub repository
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/nagaraju531/$Project_Name.git'
           }
        }
    }
}
